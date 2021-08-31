---
title: тип enum androidDeviceOwnerPlayStoreMode
description: Тип режима Play Store владельца android-устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e9b35e5d202c7d290cba2cc47c228563c7e478a8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800760"
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



