---
title: тип ресурса oemWarrantyInformationOnboarding
description: Объект состояния гарантии для данного OEM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cfa2ba539f50fe7c550fe6b22cad7d88c7e265
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292469"
---
# <a name="oemwarrantyinformationonboarding-resource-type"></a>тип ресурса oemWarrantyInformationOnboarding

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект состояния гарантии для данного OEM

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список oemWarrantyInformationOnboardings](../api/intune-devices-oemwarrantyinformationonboarding-list.md)|[коллекция oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Список свойств и связей объектов [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[Get oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-get.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Чтение свойств и связей [объекта oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[Создание oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-create.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Создайте [новый объект oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[Удаление oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-delete.md)|Нет|Удаляет [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md).|
|[Обновление oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-update.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Обновление свойств объекта [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[включить действие](../api/intune-devices-oemwarrantyinformationonboarding-enable.md)|Нет|Н/Д|
|[отключение действия](../api/intune-devices-oemwarrantyinformationonboarding-disable.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для статуса гарантии OEM. Это свойство доступно только для чтения.|
|oemName|String|Имя OEM. Это свойство доступно только для чтения.|
|enabled|Boolean|Указывает, включен ли гарантийный запрос для данного OEM. Это свойство доступно только для чтения.|
|доступен|Логическое|Указывает, доступен ли API гарантии. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oemWarrantyInformationOnboarding"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "id": "String (identifier)",
  "oemName": "String",
  "enabled": true,
  "available": true
}
```




