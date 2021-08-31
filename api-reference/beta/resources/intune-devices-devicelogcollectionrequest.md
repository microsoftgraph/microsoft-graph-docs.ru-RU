---
title: тип ресурса deviceLogCollectionRequest
description: Windows Объект запроса коллекции журналов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f23ec777fc2ff2f822210c6940c29b49bbb2a775
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791489"
---
# <a name="devicelogcollectionrequest-resource-type"></a>тип ресурса deviceLogCollectionRequest

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Объект запроса коллекции журналов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор|
|templateType|[deviceLogCollectionTemplateType](../resources/intune-devices-devicelogcollectiontemplatetype.md)|Тип шаблона, который отправляется с запросом коллекции. Возможные значения: `predefined` .|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```



