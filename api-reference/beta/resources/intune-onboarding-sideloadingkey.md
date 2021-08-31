---
title: тип ресурса sideLoadingKey
description: Объект SideLoadingKey необходим для Windows 8 и 8.1 устройств для intall Line of Business Apps для клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 651815aea6e64b4fa53f0a4d22127050c5f3b488
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792570"
---
# <a name="sideloadingkey-resource-type"></a>тип ресурса sideLoadingKey

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект SideLoadingKey необходим для Windows 8 и 8.1 устройств для intall Line of Business Apps для клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[коллекция sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Список свойств и связей [объектов sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|
|[Get sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Чтение свойств и связей [объекта sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|
|[Создание sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Создайте новый [объект sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|
|[Удаление sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|Нет|Удаляет [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[Обновление sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Обновление свойств объекта [sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный ID side Loading Key.|
|value|String|Ключевое значение side Loading — это значение 5x5, разделенное hiphens.|
|displayName|Строка|Имя клавиши боковой загрузки, отображаемой администраторам ITPro.|
|description|Строка|Описание клавиши боковой загрузки, отображаемой администраторам ITPro..|
|totalActivation|Int32|Полная активация клавиши боковой загрузки, отображаемая администраторам ITPro.|
|lastUpdatedDateTime|Строка|Клавиша side Loading Last Updated Date, отображаемая администраторам ITPro.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```



