---
title: Тип ресурса Мобилеаппдепенденци
description: Описывает тип зависимости между двумя мобильными приложениями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8140b430f8652b552c3dd2cdb85f22ba4a6190b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491762"
---
# <a name="mobileappdependency-resource-type"></a>Тип ресурса Мобилеаппдепенденци

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|таржетдисплайнаме|String|Отображаемое имя целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|депенденцитипе|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|Тип отношения зависимости между родительским и дочерним приложениями. Возможные значения: `detect`, `autoInstall`.|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения.|

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



