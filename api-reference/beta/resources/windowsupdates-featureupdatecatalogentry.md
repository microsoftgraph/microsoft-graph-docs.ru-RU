---
title: тип ресурса featureUpdateCatalogEntry
description: Метаданные для обновления Windows 10, которое можно утвердить для развертывания.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 94403127fdbc8c263df546c2dfd1359c87894a06
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861643"
---
# <a name="featureupdatecatalogentry-resource-type"></a>тип ресурса featureUpdateCatalogEntry

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Метаданные для обновления Windows 10, которое можно утвердить для развертывания.

Windows 10 обновления компонентов выпускаются раз в два года и содержат новые функции для Windows 10. Установка этих обновлений увеличивает Windows 10 сборки и, как правило, приводит к новому жизненному циклу обслуживания и концу даты службы. Корпорация Майкрософт рекомендует организациям регулярно развертывать новые обновления функций в рамках принятия Windows как услуга.

Наследует от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|Дата, в которую контент больше не доступен для развертывания с помощью службы. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|displayName|String|Отображение имени контента. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|id|String|Уникальный идентификатор для записи каталога. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|releaseDateTime|DateTimeOffset|Дата выпуска контента. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|version|String|Версия обновления функции. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "version": "String"
}
```

