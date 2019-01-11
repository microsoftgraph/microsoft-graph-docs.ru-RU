---
title: Тип ресурса administrativeUnit
description: Административное подразделение предоставляет концептуальные контейнер для пользователей и групп объектов каталога. С помощью административного единиц измерения, администратор компании теперь можно делегировать административные обязанности для управления пользователями и групп, содержащихся в рамках или заданной областью единице администрирования для администратора региональных или отделов.
localization_priority: Normal
ms.openlocfilehash: 523214d7bd319d940f042d461b4903ff1f1475e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845411"
---
# <a name="administrativeunit-resource-type"></a>Тип ресурса administrativeUnit

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Административное подразделение предоставляет концептуальные контейнер для пользователей и групп объектов каталога. С помощью административного единиц измерения, администратор компании теперь можно делегировать административные обязанности для управления пользователями и групп, содержащихся в рамках или заданной областью единице администрирования для администратора региональных или отделов.

Давайте рассмотрим пример. Предположим, что Contoso Corp состоит из двух подразделений - подразделение West регион и регион East деления. Роли каталога в домене Contoso рассматриваются в пределах всего клиента. Иванов, администратор компании Contoso, хочет делегировать административные обязанности, но ограничить область их на запад регион отдела или подразделения East регион.  Иванов можно создавать *единицы admistrative регион Запад* и поместить все пользователи West регион в такая единица.  Аналогично Иванов можно создать *единицы администрирования East регион*.  Теперь Иванов, можно начать Делегирование административных задач для других пользователей, но **областью действия** для нового административные единицы он создается. Иванов помещает Jennifer в *администратору службы поддержки* роль **областью действия** *Единица West регион*.  Это позволяет Jennifer для сброса пароля любой пользователь, но только если тех пользователей, расположенных в *Регион West единица*.  Аналогично Иванов помещает Дейв в *учетной записи администратора пользователей* роли **областью действия** *Единица East регион*.  Это позволяет Дейв обновления пользователей, назначение лицензий и сброс пароля любой пользователь, но только если эти пользователи находятся в *Регион East единица*. Видеоролик читайте [Azure Active Directory административные единиц измерения](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

В этом разделе приведены описания объявленные свойства и свойства навигации, предоставляемые administrativeUnit сущности, а также операции и функции, которые могут вызываться на administrativeUnits ресурсов.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание administrativeUnit](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Создание нового административного подразделения.|
|[Список administrativeUnits](../api/administrativeunit-list.md) | [administrativeUnit](administrativeunit.md) коллекции |Свойства списка всех administrativeUnits.|
|[Получение administrativeUnit](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Чтение свойства и связи объекта определенного administrativeUnit.|
|[Обновление adminstrativeUnit](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |Обновление объекта administrativeUnit. |
|[Удаление adminstrativeUnit](../api/administrativeunit-delete.md) | Нет |Удалите объект administrativeUnit. |
|[Добавить участника](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Добавление члена (пользователя или группы).|
|[Список членов](../api/administrativeunit-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получите список участников (пользователей и групп).|
|[Получение члена](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Получите конкретный элемент.|
|[Удаление члена](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Удалите элемент.|
|[Добавление члена области определения роли](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Добавление члена группы области определения роли.|
|[Список элементов области определения роли](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) коллекции| Получение списка администраторам области определения роли.|
|[Получение члена группы области определения роли](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Получите конкретный элемент области определения роли.|
|[Удалить члена группы области определения роли](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Удалите члена группы области определения роли.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|строка|Необязательное описание для административного подразделения.|
|displayName|строка|Отображаемое имя для административного подразделения.|
|id|строка|Уникальный идентификатор для административного подразделения. Только для чтения.|
|visibility|string|Управляет ли модульного администрирования и его члены являются скрытыми или «общедоступный». Может иметь значение HiddenMembership или «общедоступный». Если не задан, поведение по умолчанию является открытым. Если задано значение HiddenMembership, только члены административные единицы можно списка всех других членов единицы администрирования.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция open расширения, определенные для этой административные единицы. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи и группы, которые являются участниками этой единицы Adminsitrative. Методы HTTP: Получение (элементы списка), учет (добавить участников), DELETE (удалить членов).|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) коллекции| Элементы уровня роль такая единица.  Методы HTTP: Получение (список scopedRoleMemberships), учет (Добавить scopedRoleMembership), DELETE (удалить scopedRoleMembership). |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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
<!-- {
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
