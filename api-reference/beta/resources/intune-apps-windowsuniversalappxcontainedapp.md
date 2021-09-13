---
title: тип ресурса windowsUniversalAppXContainedApp
description: Класс, представляю содержащий приложение приложения WindowsUniversalAppX.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3dcdfcbe3bd61b175d9905337131e84b80a8ad82
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091834"
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
|[Получить windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Чтение свойств и связей [объекта WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Создание windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Создание нового [объекта WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Удаление windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|Нет|Удаляет [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|
|[Обновление windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Обновление свойств объекта [WindowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследованный от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|String|ID модели пользователя приложения, содержатого приложения приложения WindowsUniversalAppX.|

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



