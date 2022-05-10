---
title: Тип ресурса externalDomainName
description: Доменное имя внешней организации, с Azure Active Directory (Azure AD) в качестве клиента ресурса.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: de723382ddfdbb7ef68c871e84498560d2b03ce8
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296631"
---
# <a name="externaldomainname-resource-type"></a>Тип ресурса externalDomainName

Пространство имен: microsoft.graph

Представляет доменное имя внешней организации, с Azure Active Directory (Azure AD) в качестве клиента ресурса.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Доменное имя внешней организации, с Azure AD в федерацию с клиентом. Наследуется от [сущности](../resources/entity.md).|

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
