symbolic_status_iconsdir = join_paths(symbolic_iconsdir, 'status')

regular_files = [
    # DO NOT REMOVE: Begining of regular segment
    'TeamViewer-indicator-away.svg',
    'TeamViewer-indicator-busy.svg',
    'TeamViewer-indicator-connected.svg',
    'TeamViewer-indicator-error.svg',
    'TeamViewer-indicator-offline.svg',
    'TeamViewer-indicator.svg',
    'Zoom-indicator.svg',
    'bitwarden-tray.svg',
    'emblem-ok-symbolic.svg',
    'emblem-photos-symbolic.svg',
    'emblem-synchronizing-symbolic.svg',
    'firewall-applet-error.svg',
    'firewall-applet-panic.svg',
    'jdownloader-indicator.svg',
    'keepassxc-locked.svg',
    'keepassxc-unlocked.svg',
    'pamac-tray-no-update.svg',
    'pamac-tray-update.svg',
    'protonvpn-tray.svg',
    'protonvpngui-connected.svg',
    'protonvpngui-disconnected.svg',
    'protonvpngui-no-network.svg',
    'search-symbolic.svg',
    'solaar-attention.svg',
    'solaar-init.svg',
    'state-download.svg',
    'state-error.svg',
    'state-information.svg',
    'state-offline.svg',
    'state-ok.svg',
    'state-pause.svg',
    'state-sync.svg',
    'state-warning.svg',
    'strawberry-panel.svg',
    'sunshine-locked.svg',
    'sunshine-pausing.svg',
    'sunshine-playing.svg',
    'sunshine-tray.svg',
    'user-available.svg',
    'user-away.svg',
    'user-busy.svg',
    'user-invisible.svg',
    'user-offline.svg',
    'user-status-new.svg',
    'user-status-pending.svg',
    'vlc-panel.svg',
    # DO NOT REMOVE: End of regular segment
]

link_files = {
    # DO NOT REMOVE: Begining of link segment
    'user-status-new.svg': [
        'pidgin-tray-xa.svg',
    ],
    'user-status-pending.svg': [
        'pidgin-tray-pending.svg',
    ],
    'user-offline.svg': [
        'pidgin-tray-offline.svg',
    ],
    'user-invisible.svg': [
        'pidgin-tray-invisible.svg',
    ],
    'user-busy.svg': [
        'pidgin-tray-busy.svg',
    ],
    'user-away.svg': [
        'pidgin-tray-away.svg',
    ],
    'user-available.svg': [
        'pidgin-tray-available.svg',
        'pidgin-tray-connect.svg',
    ],
    'keepassxc-unlocked.svg': [
        'org.keepassxc.KeePassXC-unlocked.svg',
    ],
    'keepassxc-locked.svg': [
        'org.keepassxc.KeePassXC-locked.svg',
    ],
    'sunshine-tray.svg': [
        'dev.lizardbyte.app.Sunshine-tray.svg',
    ],
    'sunshine-playing.svg': [
        'dev.lizardbyte.app.Sunshine-playing.svg',
    ],
    'sunshine-pausing.svg': [
        'dev.lizardbyte.app.Sunshine-pausing.svg',
    ],
    'sunshine-locked.svg': [
        'dev.lizardbyte.app.Sunshine-locked.svg',
    ],
    'protonvpngui-no-network.svg': [
        'com.protonvpn.www.state-error.svg',
    ],
    'protonvpngui-disconnected.svg': [
        'com.protonvpn.www.state-disconnected.svg',
    ],
    'protonvpngui-connected.svg': [
        'com.protonvpn.www.state-connected.svg',
    ],
    # DO NOT REMOVE: End of link segment
}

install_data(regular_files, install_dir: symbolic_status_iconsdir)

foreach dest_file, link_files_for_dest : link_files
    foreach link_file : link_files_for_dest
        install_symlink(link_file, install_dir: symbolic_status_iconsdir, pointing_to: dest_file)
    endforeach
endforeach
