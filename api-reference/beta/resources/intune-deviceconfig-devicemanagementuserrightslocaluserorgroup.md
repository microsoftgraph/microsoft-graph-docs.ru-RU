---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a2cc0ff5b9e054398e7878b7d99619b59d109a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422063"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Тип ресурса deviceManagementUserRightsLocalUserOrGroup

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя этого локального пользователя или группы.|
|description|String|Описание администратора локального пользователя или группы.|
|Класс securityIdentifier|String|Идентификатор безопасности этого локального пользователя или группы (например * S-1-5-32-544).|

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




