---
title: Тип ресурса sideLoadingKey
description: SideLoadingKey сущность является обязательным для Windows 8 и 8.1 устройств для установите строку бизнес-приложений для клиента.
ms.openlocfilehash: cac2360e2c50e64e1b421df4efaf53802d78558b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082424"
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
|id|String|Со стороны загрузка уникальный идентификатор ключа.|
|value|String|Со стороны загрузки ключ значение — значение 5 x 5, разделенных hiphens.|
|displayName|String|Со стороны загрузка ключа имя, отображаемое для администраторов для ИТ-специалистов.|
|описание|String|Со стороны загрузки ключ описание, отображаемое для администраторов для ИТ-специалистов.|
|totalActivation|Int32|Со стороны загрузки ключ общее активация отображаются для администраторов для ИТ-специалистов.|
|lastUpdatedDateTime|String|Со стороны загрузки ключ обновлен Дата последнего отображаются для администраторов для ИТ-специалистов.|

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





