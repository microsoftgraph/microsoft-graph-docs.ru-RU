---
title: тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6122c36481204c7f6e7269839be625e45db5432a
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477484"
---
# <a name="accesspackagecatalog-resource-type"></a>тип ресурса accessPackageCatalog

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md) каталог пакетов доступа — это контейнер для пакетов с нулевым или более доступом. Управление правами Azure AD включает встроенный каталог с именем **General**.

Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для обеспечения доступа. Чтобы просмотреть или изменить членство ролей в каталоге, используйте API назначений ролей с поставщиком управления правами RBAC.[](unifiedroleassignment.md)


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [коллекция accessPackageCatalog](accesspackagecatalog.md) | Извлечение списка объектов accesspackagecatalog. |
| [Создание accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте новый объект accessPackageCatalog. |
| [Получить accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта accessPackageCatalog. |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта accessPackageCatalog. |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление accessPackageCatalog. |
| **Доступ к ресурсам пакета**| | |
| [Ресурсы accessPackageCatalog списка](../api/accesspackagecatalog-list-accesspackageresources.md) | [коллекция accessPackageResource](accesspackageresource.md) | Извлечение списка объектов accessPackageResource в каталоге. |
| **Доступ к ролям ресурсов пакета**| | |
| [Роли ресурсов accessPackageCatalog в списке](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Извлечение списка объектов accessPackageResourceRole для ресурсов в каталоге. |
| **Расширения рабочего процесса пакетов пакетов пользовательского доступа**| | |
|[Список customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-list-customaccesspackageworkflowextensions.md)|[коллекция customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Получите список объектов [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) и их свойств.|
|[Создание customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-post-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Создайте новый [объект customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Get customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-get.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Ознакомьтесь с свойствами и отношениями объекта [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Обновление customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-update.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Обновление свойств настраиваемого [объектаAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Удаление customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-delete.md)|Нет|Удаляет объект [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogStatus|Строка|Имеет значение, `Published` если пакеты доступа доступны для управления.|
|catalogType|Строка|Либо `UserManaged`, либо `ServiceDefault`. |
|createdBy|String|UPN пользователя, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание каталога пакетов доступа.|
|displayName|Строка|Отображение имени каталога пакетов доступа. Поддерживает `$filter` (`eq`, `contains`).|
|id|String| Только для чтения.|
|isExternallyVisible|Boolean|Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.|
|modifiedBy|Строка|UpN пользователя, который в последний раз изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackages|[коллекция accessPackage](accesspackage.md)| Пакеты доступа в этом каталоге. Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|accessPackageResources|[коллекция accessPackageResource](accesspackageresource.md)| Только для чтения. Допускается значение null.|
|accessPackageResourceRoles|[коллекция accessPackageResourceRole](accesspackageresourcerole.md)|Роли каждого ресурса в каталоге. Только для чтения.|
|accessPackageResourceScopes|[коллекция accessPackageResourceScope](accesspackageresourcescope.md)|Только для чтения.|
|customAccessPackageWorkflowExtension|[коллекция customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Атрибуты логического приложения, которые можно назвать на различных этапах запроса пакета доступа и цикла назначения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

