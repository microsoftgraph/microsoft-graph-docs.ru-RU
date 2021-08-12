---
title: тип ресурса конфигурации
description: Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 213c24c9388f555d772f2c0243b1d55d023239922d059b63478a8953ac6d5b25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141674"
---
# <a name="configuration-resource-type"></a>тип ресурса конфигурации

Пространство имен: microsoft.graph.externalConnectors



Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента [в externalConnection.](../resources/externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authorizedAppIds|Коллекция String|Коллекция ID-приложений для зарегистрированных Azure Active Directory приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.|

## <a name="relationships"></a>Связи
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

