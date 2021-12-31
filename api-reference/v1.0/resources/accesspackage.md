---
title: тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 226715a4678b593e68a8364e326950c7af019212
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651458"
---
# <a name="accesspackage-resource-type"></a>тип ресурса accessPackage

Пространство имен: microsoft.graph

В [Azure AD Entitlement Management](entitlementmanagement-overview.md)пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.  

Каждый пакет доступа ссылается на единый каталог пакетов доступа и имеет ссылки на ресурсы из этого каталога с помощью областей ролей, определенных ресурсами, которые определяют доступ, который предоставляет пакет.  Пакет доступа также связывается с политиками назначения пакета доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.



## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Пакеты доступа к спискам](../api/entitlementmanagement-list-accesspackages.md)|[коллекция accessPackage](accesspackage.md)|Извлечение списка **объектов accesspackage.** |
|[Создание accessPackage](../api/entitlementmanagement-post-accesspackages.md)|[accessPackage](accesspackage.md)|Создайте новый **объект accesspackage.** |
|[Получить accessPackage](../api/accesspackage-get.md)|[accessPackage](accesspackage.md)|Чтение свойств и связей объекта **accesspackage.** |
|[Обновление accessPackage](../api/accesspackage-update.md)|Нет|Обновление свойств объекта **accesspackage.** |
|[Удаление accessPackage](../api/accesspackage-delete.md)|Нет|Удаление **accesspackage**. |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[коллекция accessPackage](../resources/accesspackage.md)|Извлечение списка **объектов accessPackage,** фильтруемых на входе пользователя.|
|[getApplicablePolicyRequirements](../api/accesspackage-getapplicablepolicyrequirements.md)|[accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) collection|Извлечение списка **объектов accessPackageAssignmentRequestRequirement** с требованиями запроса. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание пакета доступа.|
|displayName|Строка|Отображение имени пакета доступа. Поддерживает $filter ( `eq` , `contains` ).|
|id|String|Только для чтения.|
|isHidden|Логический|Скрыт ли пакет доступа от запросителя.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|каталог|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isHidden": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


