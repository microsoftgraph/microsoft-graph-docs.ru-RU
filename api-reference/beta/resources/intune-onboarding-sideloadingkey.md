---
title: Тип ресурса sideLoadingKey
description: SideLoadingKey сущность является обязательным для Windows 8 и 8.1 устройств для установите строку бизнес-приложений для клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a58b835706826362e0165282234872bc77d62e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960345"
---
# <a name="sideloadingkey-resource-type"></a>Тип ресурса sideLoadingKey

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

SideLoadingKey сущность является обязательным для Windows 8 и 8.1 устройств для установите строку бизнес-приложений для клиента.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) коллекции|Свойства списка и связей объектов [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Получение sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Чтение свойства и связи объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Создание sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Создание нового объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Удаление sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|Нет|Удаляет [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[Обновление sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Обновление свойства объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Со стороны загрузка уникальный идентификатор ключа.|
|value|Строка|Со стороны загрузки ключ значение — значение 5 x 5, разделенных hiphens.|
|displayName|Строка|Со стороны загрузка ключа имя, отображаемое для администраторов для ИТ-специалистов.|
|описание|Строка|Со стороны загрузки ключ описание, отображаемое для администраторов для ИТ-специалистов.|
|totalActivation|Int32|Со стороны загрузки ключ общее активация отображаются для администраторов для ИТ-специалистов.|
|lastUpdatedDateTime|Строка|Со стороны загрузки ключ обновлен Дата последнего отображаются для администраторов для ИТ-специалистов.|

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





