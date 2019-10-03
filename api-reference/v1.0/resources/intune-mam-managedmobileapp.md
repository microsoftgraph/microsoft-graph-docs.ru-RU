---
title: Тип ресурса managedMobileApp
description: Идентификатор для развертывания приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87c10ed983db756119153baf961731f6b79a9ee3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367002"
---
# <a name="managedmobileapp-resource-type"></a>Тип ресурса managedMobileApp

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Идентификатор для развертывания приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedMobileApp](../api/intune-mam-managedmobileapp-list.md)|Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Список свойств и связей объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Получение объекта managedMobileApp](../api/intune-mam-managedmobileapp-get.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Создание объекта managedMobileApp](../api/intune-mam-managedmobileapp-create.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Удаление объекта managedMobileApp](../api/intune-mam-managedmobileapp-delete.md)|Нет|Удаляет объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Обновление объекта managedMobileApp](../api/intune-mam-managedmobileapp-update.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор приложения с типом его операционной системы.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




