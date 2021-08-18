---
title: тип enum androidDeviceOwnerPlayStoreMode
description: Тип режима Play Store владельца android-устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 62fe3b2182983c7be5f2a43f62a719d37821bfa26cb36d8c06374831a978ff8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54250051"
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
|allowList|1 |Доступны только приложения, которые находятся в политике, и любое приложение, не вписающееся в политику, будет автоматически отключаться с устройства.|
|blockList|2|Все приложения доступны, и любое приложение, которое не должно быть на устройстве, должно быть явно помечено как "ЗАБЛОКИРОВАНо" в политике приложений.|




