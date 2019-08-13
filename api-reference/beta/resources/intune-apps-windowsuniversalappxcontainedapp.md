---
title: Тип ресурса Виндовсуниверсалаппксконтаинедапп
description: Класс, представляющий вложенное приложение приложения WindowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 02ad1efef2c980bf07381ecce6f8c24203ea837e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335265"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>Тип ресурса Виндовсуниверсалаппксконтаинедапп

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, представляющий вложенное приложение приложения WindowsUniversalAppX.


Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсуниверсалаппксконтаинедаппс](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|Коллекция [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Список свойств и связей объектов [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|
|[Получение Виндовсуниверсалаппксконтаинедапп](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|Чтение свойств и связей объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|
|[Создание Виндовсуниверсалаппксконтаинедапп](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|Создание нового объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|
|[Удаление Виндовсуниверсалаппксконтаинедапп](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|Нет|Удаляет объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|
|[Обновление Виндовсуниверсалаппксконтаинедапп](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|Обновление свойств объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|
|Модели|String|ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppXContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```



