---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdb49ef0b98e3d76d092b1ebf9574d6df8c47d9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774717"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Тип ресурса Девицеманажементусерригхтслокалусерорграуп

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя локального пользователя или группы.|
|description|String|Описание локального пользователя или группы администратором.|
|Секуритидентифиер|String|Идентификатор безопасности этого локального пользователя или группы (например, * S-1-5-32-544).|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





