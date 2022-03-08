---
title: тип ресурса customCalloutExtension
description: Абстрактный тип, определяя конфигурацию логических приложений, которые могут быть интегрированы с управлением правами клиента, использует случаи для реализации более широких процессов управления. Этот абстрактный тип наследуется типом ресурса customAccessPackageWorkflowExtension
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7a76c37663fb3d9c5a49c1c539d1238d7423ba4a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339678"
---
# <a name="customcalloutextension-resource-type"></a>тип ресурса customCalloutExtension

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, определяя конфигурацию логических приложений, которые могут быть интегрированы с управлением правами клиента, использует случаи для реализации более широких процессов управления. Этот абстрактный тип наследуется типом [ресурса customAccessPackageWorkflowExtension](customaccesspackageworkflowextension.md) .

Наследуется [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|проверка подлинностиКонфигурация|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|Настройка для обеспечения безопасности вызова API в логическом приложении. Например, использование потока учетных данных клиентов OAuth. |
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)| Параметры подключения HTTP, которые определяют, как долго Azure AD может ждать подключения к логическому приложению, сколько раз можно повторить время ожидания подключения и сценарии исключений при разрешенных повторном инауки.|
|description|Строка|Описание объекта customCalloutExtension.|
|displayName|String|Отображение имени объекта customCalloutExtension.|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|Тип и сведения для настройки конечной точки для вызова рабочего процесса приложения логики.|
|id|Строка|Идентификатор для объекта customCalloutExtension. Наследуется [от сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customCalloutExtension",
  "openType": false,
  "abstract": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customCalloutExtension",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  },
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  }
}
```

