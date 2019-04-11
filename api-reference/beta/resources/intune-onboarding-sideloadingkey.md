---
title: Тип ресурса Сиделоадингкэй
description: Объект Сиделоадингкэй требуется для устройств с Windows 8 и 8,1, чтобы получить доступ к корпоративным бизнес-приложениям для клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 698d021e6038694442e5b3a6f4b3eff2a50e9943
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792127"
---
# <a name="sideloadingkey-resource-type"></a>Тип ресурса Сиделоадингкэй

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Сиделоадингкэй требуется для устройств с Windows 8 и 8,1, чтобы получить доступ к корпоративным бизнес-приложениям для клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Сиделоадингкеиес](../api/intune-onboarding-sideloadingkey-list.md)|Коллекция [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Список свойств и связей объектов [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|
|[Получение Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-get.md)|[Сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Чтение свойств и связей объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|
|[Создание Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-create.md)|[Сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Создание нового объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|
|[Удаление Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-delete.md)|Нет|Удаляет объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md).|
|[Обновление Сиделоадингкэй](../api/intune-onboarding-sideloadingkey-update.md)|[Сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Обновление свойств объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор ключа загрузки на стороне.|
|value|String|Значение ключа загрузки на стороне, это значение 5x5, разделенное хифенс.|
|displayName|String|Имя ключа загрузки на стороне, отображаемое для администраторов ИТ-специалистов.|
|description|String|Описание ключа загрузки на стороне, которое отображается для администраторов ИТ-специалистов..|
|Тоталактиватион|Int32|Клавиша загрузки на боковой стороне общая активация отображается для администраторов ИТ-специалистов.|
|lastUpdatedDateTime|String|Клавиша загрузки на боковой стороне Дата последнего обновления отображается для администраторов ИТ-специалистов.|

## <a name="relationships"></a>Отношения
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





