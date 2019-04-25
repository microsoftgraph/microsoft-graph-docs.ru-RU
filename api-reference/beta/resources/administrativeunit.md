---
title: Тип ресурса administrativeUnit
description: Административное устройство предоставляет концептуальный контейнер для объектов каталога пользователей и групп. С помощью административных единиц администратор компании может делегировать административные обязанности для управления пользователями и группами, которые находятся в административной единице или в области действия, на региональном или подразделенном администраторе.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f99fb1cd54e28aaa9526f25a0f8e09d6470df2ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535785"
---
# <a name="administrativeunit-resource-type"></a>Тип ресурса administrativeUnit

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Административное устройство предоставляет концептуальный контейнер для объектов каталога пользователей и групп. С помощью административных единиц администратор компании может делегировать административные обязанности для управления пользователями и группами, которые находятся в административной единице или в области действия, на региональном или подразделенном администраторе.

Рассмотрим эти действия на примере. Представьте, что компания Contoso Corp состоит из двух подразделений — западных и восточноазиатских подразделений. Роли каталога в компании Contoso ограничены всеми клиентами. Иванов, администратор компании Contoso, хочет делегировать административные обязанности, а область их до деления Западного или Восточного Дальневосточный.  Пользователь может создать *единицу измерения "Западный адмистративе* " и поместить все пользователи с Западом Дальневосточный в эту административную единицу.  Аналогичным образом, Иванов может создать *админстративе единицу Восточной побережье*.  Теперь можно приступить к делегированию административных обязанностей другим пользователям, но с **областью действия** , созданной для новых административных модулей, которые он создал. Иванов помещает Jennifer в роль *администратора службы поддержки* в **область** административНое подразделение Дальневосточный *Запад*.  Это позволяет Jennifer сбросить пароль любого пользователя, но только в том случае, если эти пользователи находятся в административном подразделении Дальневосточный *Запад*.  Аналогичным образом, Иванову помещаете Дениса в **** роль *администратора учетных записей пользователей* с областью *административного подразделения East Дальневосточный*.  Это позволяет Дениса обновлять пользователей, назначать лицензии и сбрасывать пароли всех пользователей, но только если они находятся в административном модуле " *Восток*". Для просмотра видео ознакомьтесь со статьей [Введение в административные единицы Azure Active Directory](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

В этом разделе описаны объявленные свойства и свойства навигации, предоставляемые объектом administrativeUnit, а также операции и функции, которые можно вызывать для ресурса Административеунитс.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание administrativeUnit](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Создайте новое административное подразделение.|
|[Список Административеунитс](../api/administrativeunit-list.md) | Коллекция [administrativeUnit](administrativeunit.md) |Список свойств всех Административеунитс.|
|[Получение administrativeUnit](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Чтение свойств и связей определенного объекта administrativeUnit.|
|[Обновление Админстративеунит](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |Обновление объекта administrativeUnit. |
|[Удаление Админстративеунит](../api/administrativeunit-delete.md) | Нет |Удаление объекта administrativeUnit. |
|[Добавить участника](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Добавление члена (пользователя или группы).|
|[Перечисление участников](../api/administrativeunit-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение списка участников (пользователей и групп).|
|[Получение члена](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Получение определенного участника.|
|[Удаление участника](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Удаление члена.|
|[Добавление роли члена с областью](../api/administrativeunit-post-scopedrolemembers.md) |[Scopedrolemembership изменен](scopedrolemembership.md)| Добавление члена с областью ролей.|
|[Область списка — элементы роли](../api/administrativeunit-list-scopedrolemembers.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| Получение списка администраторы с областью действия.|
|[Получение члена роли с областью действия](../api/administrativeunit-get-scopedrolemembers.md) |[Scopedrolemembership изменен](scopedrolemembership.md)| Получение определенного члена с областью действия роли.|
|[Удаление члена с областью ролей](../api/administrativeunit-delete-scopedrolemembers.md) |[Scopedrolemembership изменен](scopedrolemembership.md)| Удаление члена с областью ролей.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|string|Необязательное описание административной единицы.|
|displayName|строка|Отображаемое имя административной единицы.|
|id|строка|Уникальный идентификатор административной единицы. Только для чтения.|
|visibility|string|Определяет, является ли модуль админстративе и его элементы скрытыми или общедоступными. Может быть задано значение значение hiddenmembership или public. Если не задано, то поведение по умолчанию — Public. Если задано значение значение hiddenmembership, только члены административной единицы могут перечислить других членов единицы админстративе.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для данной административной единицы. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи и группы, являющиеся членами этого Админситративе подразделения. Методы HTTP: GET (List Members), POST (Add Members), DELETE (удалить участников).|
|Scopedadministrators|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Члены роли с областью действия этой административной единицы.  Методы HTTP: GET (List Скопедролемембершипс), POST (Add Scopedrolemembership изменен), DELETE (удалить Scopedrolemembership изменен). |

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/administrativeunit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
