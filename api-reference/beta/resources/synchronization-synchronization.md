---
title: тип ресурсов синхронизации
description: Представляет возможность синхронизации удостоверений Azure Active Directory Azure AD с помощью API microsoft Graph.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 9fd52e5fde2a3eee110709d0817930c0a017ee7e
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226318"
---
# <a name="synchronization-resource-type"></a>тип ресурсов синхронизации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет возможность синхронизации удостоверений Azure Active Directory Azure AD с помощью API microsoft Graph. Синхронизация удостоверений (также называемая *подготовка)* позволяет автоматизировать подготовка (создание, обслуживание) и удаление (удаление) удостоверений и ролей пользователей из Azure AD в поддерживаемые облачные приложения. Дополнительные сведения см. в [Azure Active Directory](/azure/active-directory/app-provisioning/how-provisioning-works)

## <a name="methods"></a>Методы


|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[acquireAccessToken](../api/synchronization-synchronization-acquireaccesstoken.md)|Нет| Приобрети маркер OAuth Access для авторизации службы подготовка Azure AD для обеспечения пользователей приложением. |
|[Добавление секретов](../api/synchronization-synchronization-secrets.md)|Нет| Предоставление учетных данных для установления подключения к целевой системе. |

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizations](../api/synchronization-synchronization-list.md)|[synchronization](../resources/synchronization-synchronization.md) collection|Get a list of the [synchronization](../resources/synchronization-synchronization.md) objects and their properties.|
|[Create synchronization](../api/synchronization-serviceprincipal-post-synchronization.md)|[synchronization](../resources/synchronization-synchronization.md)|Create a new [synchronization](../resources/synchronization-synchronization.md) object.|
|[Get synchronization](../api/synchronization-synchronization-get.md)|[synchronization](../resources/synchronization-synchronization.md)|Read the properties and relationships of a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Update synchronization](../api/synchronization-synchronization-update.md)|[synchronization](../resources/synchronization-synchronization.md)|Update the properties of a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Delete synchronization](../api/synchronization-synchronization-delete.md)|None|Deletes a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Ping](../api/synchronization-synchronization-ping.md)|String|**TODO: Add Description**|
|[acquireAccessToken](../api/synchronization-synchronization-acquireaccesstoken.md)|None|**TODO: Add Description**|
|[List jobs](../api/synchronization-synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronization-synchronizationjob.md) collection|Get the synchronizationJob resources from the jobs navigation property.|
|[Create synchronizationJob](../api/synchronization-synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronization-synchronizationjob.md)|Create a new synchronizationJob object.|
|[List templates](../api/synchronization-synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) collection|Get the synchronizationTemplate resources from the templates navigation property.|
|[Create synchronizationTemplate](../api/synchronization-synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)|Create a new synchronizationTemplate object.|
-->

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|секреты|[синхронизацияSecretKeyStringValuePair](synchronization-synchronizationsecretkeystringvaluepair.md) коллекция| Представляет коллекцию учетных данных для доступа к предварительным облачным приложениям.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|jobs|[коллекция synchronizationJob](../resources/synchronization-synchronizationjob.md)| Выполняет синхронизацию, периодически запущенную в фоновом режиме, опрос изменений в одном каталоге и нажатие их в другой каталог.|
|шаблоны|[коллекция synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)| Предварительно настроенные параметры синхронизации для конкретного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronization",
  "version": "String",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```

