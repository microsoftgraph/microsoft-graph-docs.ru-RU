---
title: тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователей.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb8dd01d090c5d0aaef133b5e5b6367f5acdd278
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069231"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>тип ресурса deviceManagementUserRightsLocalUserOrGroup

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователей.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя этого локального пользователя или группы.|
|description|Строка|Описание администратором этого локального пользователя или группы.|
|securityIdentifier|String|Идентификатор безопасности этого локального пользователя или группы (например, S-1-5-32-544).|

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



