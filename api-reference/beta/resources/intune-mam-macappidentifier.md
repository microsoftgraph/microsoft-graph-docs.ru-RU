---
title: Тип ресурса macAppIdentifier
description: Идентификатор приложения для Mac.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ee44dc2fe288d7a1605660ef95dc7d88f600fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160961"
---
# <a name="macappidentifier-resource-type"></a>Тип ресурса macAppIdentifier

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Идентификатор приложения для Mac.


Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleId|String|Идентификатор приложения, указанный в магазине приложений.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macAppIdentifier",
  "bundleId": "String"
}
```




