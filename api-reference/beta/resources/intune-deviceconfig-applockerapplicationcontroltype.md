---
title: тип enum appLockerApplicationControlType
description: Возможные значения типов управления приложениями AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 617db7bd086ff14611804c12506cc58b5a446d10
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791911"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>тип enum appLockerApplicationControlType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения типов управления приложениями AppLocker

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение устройства по умолчанию, не выбранный тип управления приложениями.|
|enforceComponentsAndStoreApps|1|Обеспечение Windows компонентов и хранения приложений.|
|auditComponentsAndStoreApps|2|Аудит Windows компонентов и хранения приложений.|
|enforceComponentsStoreAppsAndSmartlocker|3|Обеспечение Windows компонентов, хранения приложений и смарт-шкафчик.|
|auditComponentsStoreAppsAndSmartlocker|4 |Аудит Windows компонентов, хранения приложений и смарт-шкафчик.|



