---
title: тип ресурса customAccessPackageWorkflowExtension
description: Определяет атрибуты логического приложения, которые можно назвать на различных этапах запроса пакета доступа и цикла назначения.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b89d41ec573d6035e19590d7015df4e7269909f3
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672737"
---
# <a name="customaccesspackageworkflowextension-resource-type"></a>тип ресурса customAccessPackageWorkflowExtension

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет атрибуты логического приложения, которые можно назвать на различных этапах запроса пакета доступа и цикла назначения. Можно интегрировать логические приложения с управлением правами, чтобы расширить рабочий процесс управления за пределами основных случаев использования прав. Следующие случаи использования можно интегрировать с логическими приложениями с помощью этого рабочего процесса:
- При [запросе пакета доступа](accesspackageassignmentrequest.md)
- При [предоставлении запроса пакета доступа](accesspackageassignment.md)
- По [истечении срока назначения пакета доступа](accesspackageassignment.md)

Наследует и выводится из [customCalloutExtension](../resources/customcalloutextension.md).


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-list-customaccesspackageworkflowextensions.md)|[коллекция customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Получите список объектов [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) и их свойств.|
|[Создание customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-post-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Создайте новый [объект customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Get customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-get.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Ознакомьтесь с свойствами и отношениями объекта [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Обновление customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-update.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Обновление свойств настраиваемого [объектаAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Удаление customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-delete.md)|Нет|Удаляет объект [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|проверка подлинностиКонфигурация|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|Настройка для обеспечения безопасности вызова API в логическом приложении. Например, использование потока учетных данных клиентов OAuth. Наследуется [от customCalloutExtension](../resources/customcalloutextension.md).|
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)| Параметры подключения HTTP, которые определяют, как долго Azure AD может ждать подключения к логическому приложению, сколько раз можно повторить время ожидания подключения и сценарии исключений при разрешенных повторном инауки. Наследуется [от customCalloutExtension](../resources/customcalloutextension.md).|
|createdDateTime|DateTimeOffset|Представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание объекта customAccessPackageWorkflowExtension. Наследуется [от customCalloutExtension](../resources/customcalloutextension.md). Только для чтения.|
|displayName|Строка|Отображение имени объекта customAccessPackageWorkflowExtension. Наследуется [от customCalloutExtension](../resources/customcalloutextension.md). Только для чтения. Поддерживает `$filter` (`contains`).|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|Тип и сведения для настройки конечной точки для вызова рабочего процесса приложения логики. Наследуется [от customCalloutExtension](../resources/customcalloutextension.md).|  
|id|String|Идентификатор для объекта customAccessPackageWorkflowExtension. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customAccessPackageWorkflowExtension",
  "baseType": "microsoft.graph.customCalloutExtension",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customAccessPackageWorkflowExtension",
  "id": "String (identifier)",
  "displayName": "String",
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  },
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  }
}
```
