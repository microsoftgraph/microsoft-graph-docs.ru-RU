---
title: Тип ресурса Секуритибаселинетемплате
description: Базовый шаблон безопасности учетной записи
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8af050df4b90314ad823535860e08557075966df
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319316"
---
# <a name="securitybaselinetemplate-resource-type"></a>Тип ресурса Секуритибаселинетемплате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый шаблон безопасности учетной записи


Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритибаселинетемплатес](../api/intune-deviceintent-securitybaselinetemplate-list.md)|Коллекция [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md)|Список свойств и связей объектов [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Получение Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Чтение свойств и связей объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Создание Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Создание нового объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Удаление Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|Нет|Удаляет объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md).|
|[Обновление Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Обновление свойств объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|Строка|Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|String|Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|String|Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|нерекомендуемый|Boolean|Шаблон устарел или не является устаревшим. Не удается создать объект "удержания" из устаревшего шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|интенткаунт|Int32|Количество целей, созданных на основе этого шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|TemplateType — тип|[девицеманажементтемплатетипе](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|Тип шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.|
|publishedDateTime|DateTimeOffset|При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|settings|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция всех параметров, унаследованных этим шаблоном от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|categories|Коллекция [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Коллекция параметров категорий в шаблоне, унаследованных от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|мигратаблето|Коллекция [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|Коллекция шаблонов, которые можно перенести в шаблон, наследуемый от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|девицестатесуммари|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Сводка по состоянию базового устройства безопасности|
|deviceStates|Коллекция [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Состояния основного устройства безопасности|
|категоридевицестатесуммариес|Коллекция [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Базовый план безопасности для категории "Сводка по состоянию устройства"|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "publishedDateTime": "String (timestamp)"
}
```



