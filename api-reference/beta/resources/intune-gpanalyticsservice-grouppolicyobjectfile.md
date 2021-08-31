---
title: тип ресурса groupPolicyObjectFile
description: Объектный файл групповой политики, загруженный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e02d93e37e83c462a5eb15435dc41e69c886d9ca
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816489"
---
# <a name="grouppolicyobjectfile-resource-type"></a>тип ресурса groupPolicyObjectFile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объектный файл групповой политики, загруженный администратором.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyObjectFiles](../api/intune-gpanalyticsservice-grouppolicyobjectfile-list.md)|[коллекция groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Список свойств и связей объектов [groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|
|[Get groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Чтение свойств и связей объекта [groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|
|[Создание groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-create.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Создайте новый [объект groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|
|[Удаление groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-delete.md)|Нет|Удаляет [группуPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).|
|[Update groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-update.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Обновление свойств объекта [groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|groupPolicyObjectId|Guid|GUID объекта групповой политики из контента GPO Xml|
|ouDistinguishedName|String|Отличительное имя OU.|
|createdDateTime|DateTimeOffset|Дата и время, в которые была впервые загружена GroupPolicy.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyObjectFile.|
|content|String|Контент объекта групповой политики.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "content": "String"
}
```



