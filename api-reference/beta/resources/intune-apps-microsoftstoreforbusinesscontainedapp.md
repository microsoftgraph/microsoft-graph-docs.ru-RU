---
title: Тип ресурса microsoftStoreForBusinessContainedApp
description: Класс, представляющий автономные приложения из MicrosoftStoreForBusinessApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef58e406a7c7524e3212546b4c10e6874078277
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395610"
---
# <a name="microsoftstoreforbusinesscontainedapp-resource-type"></a>Тип ресурса microsoftStoreForBusinessContainedApp

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, представляющий автономные приложения из MicrosoftStoreForBusinessApp.


Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftStoreForBusinessContainedApps](../api/intune-apps-microsoftstoreforbusinesscontainedapp-list.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) коллекции|Свойства списка и связей объектов [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|
|[Получение microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-get.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md);|Чтение свойства и связи объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|
|[Создание microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-create.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md);|Создание нового объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|
|[Удаление microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-delete.md)|Нет|Удаляет [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).|
|[Обновление microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-update.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md);|Обновление свойства объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|String|Автономные приложения MicrosoftStoreForBusinessApp модели пользователя приложения.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```




