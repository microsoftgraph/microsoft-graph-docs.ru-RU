---
title: Тип ресурса удостоверений
description: Удостоверение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cac61a828f7d602bfd0bb0775e35f323ba0d491e
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60486837"
---
# <a name="identity-resource-type"></a>Тип ресурса удостоверений

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Удостоверение

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор удостоверения. Это свойство доступно только для чтения.|
|displayName|String|Отображение имени удостоверения. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identity",
  "id": "String (identifier)",
  "displayName": "String"
}
```



