---
title: тип enum androidDeviceOwnerPlayStoreMode
description: Тип режима Play Store владельца android-устройства.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d7110a4dcc255e47866b3746273d6a87c670f12e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106576"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a>тип enum androidDeviceOwnerPlayStoreMode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип режима Play Store владельца android-устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Not Configured|
|allowList|1|Доступны только приложения, которые находятся в политике, и любое приложение, не вписающееся в политику, будет автоматически отключаться с устройства.|
|blockList|2|Все приложения доступны, и любое приложение, которое не должно быть на устройстве, должно быть явно помечено как "ЗАБЛОКИРОВАНо" в политике приложений.|



