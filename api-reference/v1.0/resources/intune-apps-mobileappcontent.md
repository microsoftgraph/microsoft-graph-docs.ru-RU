---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae87e5a926493c46cc7b51ac2c0bd67a802ddbcf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109061"
---
# <a name="mobileappcontent-resource-type"></a>Тип ресурса mobileAppContent

Пространство имен: microsoft.graph

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
|id|Строка|Версия контента приложения.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|files|Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Список файлов для этой версии контента приложения.|

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




