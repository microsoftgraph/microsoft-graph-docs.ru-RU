---
title: Тип ресурса Виндовсуниверсалаппксконтаинедапп
description: Класс, представляющий вложенное приложение приложения WindowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff3f5b074d0a88c93fadd52c48059b73e6a82506
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558365"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>Тип ресурса Виндовсуниверсалаппксконтаинедапп

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, представляющий вложенное приложение приложения WindowsUniversalAppX.


НаСледуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)

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
|id|String|Ключ объекта. НаСледуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|
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





