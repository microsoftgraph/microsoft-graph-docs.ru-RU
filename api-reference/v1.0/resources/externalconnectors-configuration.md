---
title: тип ресурса конфигурации
description: Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2d7955887a999b6e46d8af77b5da47358e20c2f2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123470"
---
# <a name="configuration-resource-type"></a>тип ресурса конфигурации

Пространство имен: microsoft.graph.externalConnectors



Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента [в externalConnection.](../resources/externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authorizedAppIds|Коллекция String|Коллекция ID-приложений для зарегистрированных Azure Active Directory приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.configuration"
}
-->
``` json
{
  "authorizedAppIds": [
    "String"
  ]
}
```

