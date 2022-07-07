---
title: Тип перечисления appManagementLevel
description: Уровни управления для приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d97b5973842d281dc8631a92c6818cb1d7026ae
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669023"
---
# <a name="appmanagementlevel-enum-type"></a>Тип перечисления appManagementLevel

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Уровни управления для приложений

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Неопределенное|0|Не определено.|
|Неуправляемые|1|Неуправляемые|
|Mdm|2|MDM|
|androidEnterprise|4|Android Enterprise|
|androidEnterpriseDedicatedDevicesWithAzureAdSharedMode|8 |Выделенные устройства Android Enterprise с Azure AD режимом общего доступа|
|androidOpenSourceProjectUserAssociated|16|Устройства Android с открытым исходным кодом (AOSP)|
|androidOpenSourceProjectUserless|32|Устройства android Open Source Project (AOSP) без пользователей|




