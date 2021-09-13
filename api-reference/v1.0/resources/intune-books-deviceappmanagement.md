---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8a137ac9a1d40e6eeb7d46c839c4d883b1c31a6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136602"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune-books-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-books-deviceappmanagement.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-books-deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune-books-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-books-deviceappmanagement.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune-books-deviceappmanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|managedEBooks|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Управляемая электронная книга.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




