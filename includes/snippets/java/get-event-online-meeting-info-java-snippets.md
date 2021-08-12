---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ecc018e40c056173bee17c0031a9df942e7e00becbdd5614a71af4b06bd2c01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240555"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().events("AAMkADAGu0AABIGYDZAAA=")
    .buildRequest()
    .select("isOnlineMeeting,onlineMeetingProvider,onlineMeeting")
    .get();

```