---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bf4ac6aa9de235b1e4117b47c6a5eafc5c011a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332752"
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
|секуритидентифиер|String|Идентификатор безопасности этого локального пользователя или группы (например, * S-1-5-32-544).|

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



