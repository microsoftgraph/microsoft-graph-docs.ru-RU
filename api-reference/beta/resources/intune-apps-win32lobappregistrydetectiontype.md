---
title: тип enum win32LobAppRegistryDetectionType
description: Содержит все поддерживаемые типы обнаружения данных реестра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 11ca5cf3e734a2d707547e3d50e0bc91d9b16e99b3d76ac302156fa4f5c6d810
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165842"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>тип enum win32LobAppRegistryDetectionType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит все поддерживаемые типы обнаружения данных реестра.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Не настроен.|
|существует|1 |Указанный ключ реестра или значение существует.|
|doesNotExist|2|Указанного ключа или значения реестра не существует.|
|string|3 |Тип значения строки.|
|integer|4 |Тип значения Integer.|
|version|5 |Тип значения версии.|




