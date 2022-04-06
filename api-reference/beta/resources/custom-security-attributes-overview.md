---
title: Обзор пользовательских атрибутов безопасности с помощью microsoft API Graph (Preview)
description: Узнайте, как программным образом определить собственные атрибуты безопасности и назначить их объектам Azure AD с помощью microsoft API Graph.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: conceptualPageType
ms.openlocfilehash: 609e92333195f883ed8387320f925255654fa5ad
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607759"
---
# <a name="overview-of-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>Обзор пользовательских атрибутов безопасности с помощью microsoft API Graph (Preview)

> [!IMPORTANT]
> Функция пользовательских атрибутов безопасности в настоящее время находится в режиме Предварительного просмотра. Дополнительные термины использования для [Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) для юридических терминов, применимых к функциям Azure, которые находятся в бета-версии, предварительной версии или еще не выпущены в общую доступность.

[Настраиваемые](/azure/active-directory/fundamentals/custom-security-attributes-overview) атрибуты безопасности в Azure Active Directory (Azure AD) — это бизнес-атрибуты (пары значений ключей), которые можно определить и назначить объектам Azure AD. Эти атрибуты можно использовать для хранения информации, классификации объектов или обеспечения контроля над конкретными ресурсами Azure. Настраиваемые атрибуты безопасности можно использовать с помощью управления доступом на основе атрибутов [Azure (Azure ABAC)](/azure/role-based-access-control/conditions-overview).

В этой статье представлен обзор использования microsoft API Graph для программных определений и назначения собственных атрибутов безопасности.

## <a name="key-resource-types"></a>Ключевые типы ресурсов

Ниже приводится создание блоков пользовательских атрибутов безопасности.

### <a name="attribute-sets"></a>Наборы атрибутов

Набор *атрибутов* — это группа связанных пользовательских атрибутов безопасности. Ниже 100 000. Общие характеристики наборов атрибутов:

+ Имя не может включать пробелы или специальные символы.
+ Нельзя переименовать или удалить.
+ Можно делегировать другим пользователям для определения и назначения пользовательских атрибутов безопасности.

Чтобы настроить наборы атрибутов, используйте [тип ресурса attributeSet](attributeset.md).
 
### <a name="custom-security-attribute-definitions"></a>Пользовательские определения атрибутов безопасности

*Настраиваемый атрибут безопасности —* это схема настраиваемого атрибута безопасности или пары значений ключа. Например, имя атрибута настраиваемой безопасности, описание, тип данных и предопределяемые значения. Ниже 100. Общие характеристики определений атрибутов настраиваемой безопасности:

+ Имя не может включать пробелы или специальные символы.
+ Нельзя переименовать или удалить, но можно отключить.
+ Должно быть частью набора атрибутов.

Чтобы настроить настраиваемые определения атрибутов безопасности, используйте [тип ресурса customSecurityAttributeDefinition](customsecurityattributedefinition.md).

### <a name="allowed-values"></a>Допустимые значения

*Допустимые значения* представляют предопределяемые значения настраиваемого атрибута безопасности. Ниже 100. Общие характеристики разрешенных значений:

+ Значения могут включать пробелы, но некоторые специальные символы не допускаются.
+ Нельзя переименовать или удалить, но можно отключить.
+ Дополнительные предопределяемые значения можно добавить позже.
+ Может иметь типы данных Boolean, Integer или String.

Чтобы настроить допустимые значения, используйте [допустимый тип ресурсаValue](allowedvalue.md).

## <a name="which-directory-objects-support-custom-security-attributes"></a>Какие объекты каталога поддерживают настраиваемые атрибуты безопасности?

Настраиваемые атрибуты безопасности могут быть назначены следующим объектам с помощью `customSecurityAttributes` свойства. Синхронизированным пользователям каталога из локальная служба Active Directory также могут быть назначены настраиваемые атрибуты безопасности.

+ [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
+ [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)

## <a name="limits-and-constraints"></a>Ограничения и ограничения

Список ограничений и ограничений для настраиваемого атрибута безопасности см. в списке [Ограничения и ограничения](/azure/active-directory/fundamentals/custom-security-attributes-overview#limits-and-constraints).

## <a name="permissions"></a>Permissions

Чтобы управлять настраиваемой атрибутами безопасности, основной вызов должен быть назначен одной из следующих ролей Azure AD. По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

+ [Считыватель определения атрибутов](/azure/active-directory/roles/permissions-reference#attribute-definition-reader)
+ [Администратор определения атрибутов](/azure/active-directory/roles/permissions-reference#attribute-definition-administrator)
+ [Чтение назначений атрибутов](/azure/active-directory/roles/permissions-reference#attribute-assignment-reader)
+ [Администратор назначения атрибутов](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

Кроме того, директору по вызову должны быть предоставлены соответствующие пользовательские атрибуты [безопасности](/graph/permissions-reference#custom-security-attributes-permissions).

## <a name="license-requirements"></a>Требования лицензирования

Использование настраиваемой атрибуты безопасности требует лицензии Azure AD Premium P1 или P2.

## <a name="next-steps"></a>Дальнейшие действия

+ [тип ресурса customSecurityAttributeDefinition](/graph/api/resources/customsecurityattributedefinition)
+ [Назначение, обновление или удаление настраиваемой атрибуты безопасности с помощью microsoft API Graph](/graph/custom-security-attributes-examples)
+ [Что такое настраиваемые атрибуты безопасности в Azure AD?](/azure/active-directory/fundamentals/custom-security-attributes-overview)

