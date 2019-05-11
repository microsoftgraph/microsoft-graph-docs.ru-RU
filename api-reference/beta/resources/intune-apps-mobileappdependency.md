---
title: Тип ресурса Мобилеаппдепенденци
description: Описывает тип зависимости между двумя мобильными приложениями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf64854db4421028d4982145a860141a7dc91f61
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949936"
---
# <a name="mobileappdependency-resource-type"></a>Тип ресурса Мобилеаппдепенденци

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает тип зависимости между двумя мобильными приложениями.


Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список МобилеаппдепенденЦиес](../api/intune-apps-mobileappdependency-list.md)|Коллекция [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md)|Список свойств и связей объектов [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .|
|[Получение Мобилеаппдепенденци](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Чтение свойств и связей объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .|
|[Создание Мобилеаппдепенденци](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .|
|[Удаление Мобилеаппдепенденци](../api/intune-apps-mobileappdependency-delete.md)|Нет|Удаляет объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md).|
|[Обновление Мобилеаппдепенденци](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Обновление свойств объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Строка|Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|Таржетдисплайнаме|Строка|Отображаемое имя целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|Депенденцитипе|[Мобилеаппдепенденцитипе](../resources/intune-apps-mobileappdependencytype.md)|Тип отношения зависимости между родительским и дочерним приложениями. Возможные значения: `detect`, `autoInstall`.|
|Депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```




