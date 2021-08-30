---
title: тип ресурса externalDomainName
description: Доменное имя внешней организации Azure Active Directory клиент Azure AD, выступая в качестве клиента ресурса, пытается настроить федерацию.
author: namkedia
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a84c13d4800d79263ef63423ef390846eecb5ec2
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697055"
---
# <a name="externaldomainname-resource-type"></a>тип ресурса externalDomainName

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет доменное имя внешней организации, с помощью Azure Active Directory (Azure AD), действующей в качестве клиента ресурса, пытается настроить федерацию.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Доменное имя внешней организации, которую федерирует клиент Azure AD. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalDomainName",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalDomainName",
  "id": "String (identifier)"
}
```
