---
title: Тип ресурса Сиделоадингкэй
description: Объект Сиделоадингкэй требуется для устройств с Windows 8 и 8,1, чтобы получить доступ к корпоративным бизнес-приложениям для клиента.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1a5f0dbc305e7a9cd71cfb8a90046edf1e2cfb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777940"
---
# <a name="sideloadingkey-resource-type"></a>Тип ресурса Сиделоадингкэй

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Сиделоадингкэй требуется для устройств с Windows 8 и 8,1, чтобы получить доступ к корпоративным бизнес-приложениям для клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Сиделоадингкеиес](../api/intune-onboarding-sideloadingkey-list.md)|Коллекция [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Список свойств и связей объектов [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|
|[Получение Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-get.md)|[сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Чтение свойств и связей объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|
|[Создание Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-create.md)|[сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Создание нового объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|
|[Удаление Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-delete.md)|Нет|Удаляет объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md).|
|[Обновление Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-update.md)|[сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Обновление свойств объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор ключа загрузки на стороне.|
|value|String|Значение ключа загрузки на стороне, это значение 5x5, разделенное хифенс.|
|displayName|Строка|Имя ключа загрузки на стороне, отображаемое для администраторов ИТ-специалистов.|
|description|String|Описание ключа загрузки на стороне, которое отображается для администраторов ИТ-специалистов..|
|тоталактиватион|Int32|Клавиша загрузки на боковой стороне общая активация отображается для администраторов ИТ-специалистов.|
|lastUpdatedDateTime|String|Клавиша загрузки на боковой стороне Дата последнего обновления отображается для администраторов ИТ-специалистов.|

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



