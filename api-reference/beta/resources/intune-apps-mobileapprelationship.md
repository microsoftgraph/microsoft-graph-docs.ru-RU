---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3841ab8e10bb1306dcd2f7b5b3002ded0bd2fcbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491430"
---
# <a name="mobileapprelationship-resource-type"></a>Тип ресурса Мобилеаппрелатионшип

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеаппрелатионшипс](../api/intune-apps-mobileapprelationship-list.md)|Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .|
|[Получение Мобилеаппрелатионшип](../api/intune-apps-mobileapprelationship-get.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности отношения.|
|targetId|String|Идентификатор приложения целевого дочернего мобильного приложения.|
|таржетдисплайнаме|String|Отображаемое имя целевого дочернего мобильного приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String"
}
```



