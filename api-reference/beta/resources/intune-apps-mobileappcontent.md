---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82c2100fb7bd9e906bf6cf9092d3df88865c26e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153447"
---
# <a name="mobileappcontent-resource-type"></a>Тип ресурса mobileAppContent

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppContents](../api/intune-apps-mobileappcontent-list.md)|Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Получение объекта mobileAppContent](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md);|Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Создание объекта mobileAppContent](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md);|Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Удаление объекта mobileAppContent](../api/intune-apps-mobileappcontent-delete.md)|Нет|Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Обновление объекта mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Версия контента приложения.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|files|Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Список файлов для этой версии контента приложения.|
|containedApps|Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




