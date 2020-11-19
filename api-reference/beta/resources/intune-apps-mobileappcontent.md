---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd09faa187f6621f07d2811a90ca706a6da24db6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281070"
---
# <a name="mobileappcontent-resource-type"></a>Тип ресурса mobileAppContent

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppContents](../api/intune-apps-mobileappcontent-list.md)|Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Получение объекта mobileAppContent](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Создание объекта mobileAppContent](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Удаление объекта mobileAppContent](../api/intune-apps-mobileappcontent-delete.md)|Нет|Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Обновление объекта mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Версия контента приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
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




