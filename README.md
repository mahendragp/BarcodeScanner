# BarcodeScanner

A powerful, fast and efficient library to scan Barcode and QR Codes. Min. iOS requirement is iOS 10.0

How to use...

    let vc = MGPScannerViewController.viewControllerFrom(storyboard: "Main", withIdentifier: "MGPScannerViewController")!
    vc.delegate = self 
    vc.closeBarButtonDirection = .right // to dismiss/pop view controller
    vc.overlayColor = UIColor.yellow // color if lines over camera

    vc.closeBarButton = UIBarButtonItem(title: "Close", style: .done, target: self, action: #selector(close)) // cutomise bar button item

    let nav = UINavigationController(rootViewController: vc)
    nav.navigationBar.tintColor = UIColor.whit
    nav.navigationBar.barTintColor = UIColor.brown
    present(nav, animated: true, completion: nil)
    
    
Any suggessions are most welcome.
