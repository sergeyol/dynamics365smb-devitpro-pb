---
title: "Choosing Runtime Version in AL"
description: "How to choose runtime in AL for Business Central."
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 10/01/2021
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: conceptual
ms.service: "dynamics365-business-central"
ms.author: solsen
---

# Choosing Runtime Version in AL

The capabilities and features of AL for [!INCLUDE[prod_short](../includes/prod_short.md)] are determined by the runtime version. The runtime version can be specified in the `app.json` file for a project. It is expressed with the following syntax, for example: `"runtime": "7.0"`. Specifying the runtime version is mostly interesting for scenarios where you develop for on-prem or a mix of on-prem and SaaS. For SaaS only development, you will most likely be interested in using the current runtime. If the runtime setting is not specified, the compiler will detect the runtime that matches the server.

The runtime version specified in the `app.json` file determines which runtime the project is targeting. A project can be published to the server with an earlier or with the same runtime version as the server. 

## Currently available runtime versions

The available options for setting the `runtime` in AL are:

|Runtime version|Shipped with                       |
|---------------|-----------------------------------|
|`1.0`          |Business Central April 2018 Release|
|`2.0`          |Business Central Fall '18 Release  |
|`3.0`          |Business Central Spring '19 Release|
|`4.0`          |Business Central 2019 release wave 2|
|`5.0`          |Business Central 2020 release wave 1|
|`6.0`          |Business Central 2020 release wave 2|
|`6.1`          |Business Central 2020 release wave 2 update 17.1|
|`6.2`          |Business Central 2020 release wave 2 update 17.2|
|`6.3`          |Business Central 2020 release wave 2 update 17.3|
|`6.4`          |Business Central 2020 release wave 2 update 17.4|
|`7.0`          |Business Central 2021 release wave 1|
|`7.1`          |Business Central 2021 release wave 1 update 18.1|
|`7.2`          |Business Central 2021 release wave 1 update 18.2|
|`8.0`          |Business Central 2021 release wave 2|

## Setting the runtime version

Selecting the runtime depends on the circumstances. If you, for example, have customers that run on older versions, you should set the runtime to be the minimum version that works to ensure compatibility. This will prevent you from inadvertently using features that are not supported on the older server.

If an earlier runtime is picked, it can be good idea to have a daily or weekly build that tests the extension against the latest version of the runtime. Testing against the latest runtime can detect new diagnostics, such as warnings or errors, that are introduced in the compiler or changes in the platform runtime. Though it may not be possible to refactor code for a future runtime, while using an older runtime, staying on top of these changes may help making design decisions early on.

## See Also

[JSON Files](devenv-json-files.md)  