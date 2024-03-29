---
title: Обзор API методов проверки подлинности приложений Azure AD
description: Методы проверки подлинности приложений позволяют приложениям приобретать маркеры для доступа к данным в Azure AD.
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 8c89a07cae63959904d902ae96ffb886f4877cda
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334116"
---
# <a name="azure-ad-application-authentication-methods-api-overview-preview"></a>Обзор API методов проверки подлинности приложений Azure AD (предварительный просмотр)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Методы проверки подлинности приложений, такие как сертификаты и секреты паролей, позволяют приложениям приобретать маркеры для доступа к данным в Azure Active Directory (Azure AD). Политики позволяют ИТ-администраторам применять лучшие практики использования приложениями в их организациях этих методов проверки подлинности приложений. Например, администратор может настроить политику, чтобы заблокировать использование или ограничить срок службы секретов паролей, а также использовать дату создания объекта для применения политики.

Эти политики позволяют организациям воспользоваться новыми функциями затвердения безопасности приложений. Применяя ограничения, основанные на дате создания основного приложения или службы, организация может просмотреть текущую осанку безопасности приложений, приложения инвентаризации и обеспечить соблюдение элементов управления в зависимости от их графиков и потребностей. Такой подход с использованием созданной даты позволяет организации применять политику для новых приложений, а также применять ее к существующим приложениям.

Существует два типа элементов управления политикой:

- Политика по умолчанию клиента, применяемая ко всем приложениям или директорам служб.
- Политики управления приложениями (основными приложениями или службами), которые позволяют включить или исключить отдельные приложения из политики по умолчанию клиента.

## <a name="tenant-default-app-management-policy"></a>Политика управления приложениями по умолчанию для клиента

Политика по умолчанию клиента — это единственный объект, который всегда существует и отключен по умолчанию. Он определяется ресурсом [tenantAppManagementPolicy](tenantappmanagementpolicy.md) и применяет ограничения для основных объектов приложения и службы. Он содержит следующие два свойства:

- **applicationRestrictions** позволяет нацелить приложения, которые принадлежат клиенту (объекты приложений).
- **servicePrincipalRestrictions** позволяет нацелить на нее, задаваемую от другого клиента (основные объекты службы.

Эти свойства позволяют организации либо заблокировать приложения, которые происходят в клиенте, либо повысить планку качества для приложений, которые будут за пределами границы клиента.

## <a name="app-management-policy-for-applications-and-service-principals"></a>Политика управления приложениями для приложений и директоров служб

Политики управления приложениями определяются в ресурсе [appManagementPolicy](appmanagementpolicy.md) , который содержит коллекцию политик с различными ограничениями или различными датами выполнения, которые отличаются от того, что определено в политике по умолчанию клиента. Одна из этих политик может быть назначена директору приложения или службы, исключая их из политики по умолчанию клиента.

Когда существует политика по умолчанию клиента и политика управления приложениями, политика управления приложениями имеет приоритет, а назначенное приложение или руководитель службы не наследует политику по умолчанию клиента. Только одна политика может быть назначена директору приложения или службы.

> [!Note]
> Ни политики по умолчанию клиента, ни политики управления приложениями не блокируют выдачу маркеров для существующих приложений. Приложение, которое не соответствует требованиям политики, будет работать до тех пор, пока оно не попытается обновить ресурс, чтобы добавить новый секрет.

## <a name="what-restrictions-can-be-managed-in-microsoft-graph"></a>Какие ограничения можно управлять в Microsoft Graph?

API политики проверки подлинности приложений предлагает следующие ограничения:

| Имя ограничения       | Описание                                                            | Примеры                                                                                                    |
| :--------------------- | :--------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------- |
| passwordAddition       | Ограничить секреты паролей в приложениях.                  | Блокировка новых паролей в приложениях, созданных в "01.01.2019".                                       |
| passwordLifetime       | Соблюдение максимального диапазона срока службы для секрета пароля.                    | Ограничить все новые секреты паролей максимум 30 днями для приложений, созданных после 01.01.2015 г.        |
| customPasswordAddition | Ограничение секрета пользовательского пароля в приложении или основной службе. | Ограничить все новые пользовательские (не созданные Azure AD) секреты паролей в приложениях, созданных после 01.01.2015. |
| symmetricKeyAddition   | Ограничить симметричные клавиши в приложениях.                               | Блокировка новых симметричных ключей в приложениях, созданных в 01.01.2019 или после него.                                    |
| symmetricKeyLifetime   | Соблюдение максимального диапазона срока службы для симметричного ключа.                      | Ограничение всех новых симметричных ключей до 30 дней для приложений, созданных после 01.01.2019 г.          |
| asymmetricKeyLifetime  | Соблюдение максимального диапазона срока службы для асимметричного ключа (сертификата).      | Ограничение всех новых секретов асимметричных ключей максимум до 30 дней для приложений, созданных после 01.01.2019 г.  |

> [!Note]
> Все ограничения срока службы выражены в формате isO-8601 (например: P4DT12H30M5S).
>
> Применение ограничения **customPasswordAddition** блокирует любые устаревшие модули PowerShell, которые добавляют секрет пароля, созданный клиентом, в приложения или главные службы. Это ограничение не блокирует секреты приложений или основных паролей службы, созданных Azure AD.

### <a name="single-vs-multi-tenant-apps"></a>Одноместные и многоканавтные приложения

В зависимости от того, является ли ваше приложение одним клиентом или многотенантным приложением, политика применяется к приложению или основному объекту службы следующим образом:

- Для приложений одного клиента применяем политику к объекту приложения.
- Чтобы ограничить использование приложений с несколькими клиентами, установленных в клиенте, применить политику к объекту приложения.
- Чтобы ограничить использование нескольких клиентных приложений от другого клиента, применяем политику к основному объекту службы.

### <a name="summary-of-key-differences-between-the-tenant-default-policy-and-app-management-policies"></a>Сводка основных различий между политикой по умолчанию клиента и политиками управления приложениями

| Политика по умолчанию клиента                                                              | Политика управления приложениями                                                                                                                               |
| ---------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| Политика всегда существует.                                                              | Объекты политики можно создавать или обновлять для переопределения политики по умолчанию.                                                                                |
| Ограничения отключены по умолчанию для приложения/SP.                                   | Позволяет настраивать для одного клиента или нескольких клиентов (приложение для подстройки в домашнем клиенте или в предварительном приложении).                                             |
| Разрешает только одно определение объекта ограничения для всех ресурсов.                | Позволяет определить несколько объектов политики, но только один может быть применен к ресурсу.                                                            |
| Позволяет различать ограничения для объектов приложений и принципов службы. | Политика может применяться либо к объекту приложения, либо к основному объекту службы.                                                                         |
| Применяет все ограничения, настроенные ко всем приложениям или директорам служб.             | Применяет только ограничения, настроенные в политике ресурсов, к указанному приложению или директору службы и не наследует политику по умолчанию. |

## <a name="next-steps"></a>Дальнейшие действия

- [тип ресурса tenantAppManagementPolicy](tenantappmanagementpolicy.md) .
- [тип ресурса appManagementPolicy](appmanagementpolicy.md) .
