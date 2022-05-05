---
title: Тип ресурса zebraFotaArtifact
description: Описывает один артефакт для конкретной модели устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cea341ecb1d3151e8e4f895f6038b7f47cb95cba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213551"
---
# <a name="zebrafotaartifact-resource-type"></a>Тип ресурса zebraFotaArtifact

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает один артефакт для конкретной модели устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов zebraFotaArtifacts](../api/intune-androidfotaservice-zebrafotaartifact-list.md)|[Коллекция zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Список свойств и связей объектов [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|
|[Получение объекта zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-get.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Чтение свойств и связей объекта [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|
|[Создание объекта zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-create.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Создайте объект [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|
|[Удаление объекта zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-delete.md)|Нет|Удаляет объект [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md).|
|[Обновление zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-update.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Обновление свойств объекта [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор ZebraFotaArtifact.|
|deviceModel|String|Модель артефакта устройства.|
|osVersion|String|Версия ОС артефакта.|
|patchVersion|Строка|Версия исправления артефакта.|
|boardSupportPackageVersion|Строка|Версия пакета поддержки Board.|
|releaseNotesUrl|Строка|URL-адрес заметок о выпуске артефакта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaArtifact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "id": "String (identifier)",
  "deviceModel": "String",
  "osVersion": "String",
  "patchVersion": "String",
  "boardSupportPackageVersion": "String",
  "releaseNotesUrl": "String"
}
```




