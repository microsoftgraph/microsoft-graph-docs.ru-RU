---
title: тип ресурса windowsUniversalAppXContainedApp
description: Класс, представляю содержащий приложение приложения WindowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3560ffe1584f22c7754d602e1da1564b12e88f6e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806091"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>тип ресурса windowsUniversalAppXContainedApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, представляю содержащий приложение приложения WindowsUniversalAppX.


Наследует от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsUniversalAppXContainedApps](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|[коллекция windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Список свойств и связей объектов [WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Получить windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|Чтение свойств и связей [объекта WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Создание windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|Создание нового [объекта WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Удаление windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|Нет|Удаляет [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|
|[Обновление windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|Обновление свойств объекта [WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Унаследованный от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|Строка|ID модели пользователя приложения, содержатого приложения приложения WindowsUniversalAppX.|

## <a name="relationships"></a>Связи
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



