---
title: тип enum appLockerApplicationControlType
description: Возможные значения типов управления приложениями AppLocker
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 17eb373368fe59391c9a19f7dbd91397d727e770
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081369"
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



