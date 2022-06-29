---
title: Обзор API для личных контактов Outlook
description: Используйте API личных контактов Outlook в Microsoft Graph для управления электронной почтой, планирования собраний, поиска сведений о пользователях, обмена файлами и совместной работы в группах.
author: angelgolfer-ms
ms.localizationpriority: high
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 95a66efaab47cdc178b81a5e5d4167d708e51d31
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447102"
---
# <a name="outlook-personal-contacts-api-overview"></a>Обзор API для личных контактов Outlook

Контакты Outlook позволяют хранить данные личных контактов и являются частью центра обмена сообщениями Outlook в Microsoft 365. Через Outlook можно управлять сообщениями электронной почты, планировать собрания, искать сведения о пользователях организации, начинать беседы в Интернете, делиться файлами и совместно работать в группах.

## <a name="why-integrate-with-outlook-personal-contacts"></a>Для чего выполнять интеграцию с личными контактами Outlook?

### <a name="complement-messaging-and-calendaring-scenarios-for-hundreds-of-millions-of-customers"></a>Расширение сценариев обмена сообщениями и ведения календаря для сотен миллионов клиентов

Сотни миллионов потребителей и десятки миллионов организаций выбирают Outlook в качестве своего почтового клиента. Контакты используются как дополнение к обмену сообщениями и ведению календаря, позволяя клиентам хранить данные контактов в Outlook. Для разработчиков, получивших доступ к богатому функционалу [почты](outlook-mail-concept-overview.md) или [календаря](outlook-calendar-concept-overview.md), открывается возможность создания более сложных сценариев с использованием данных о контактах пользователя.

### <a name="automate-contact-organization"></a>Автоматизация организации контактов

API контактов позволяет упорядочивать ваших клиентов аналогично тому, как это делают в Outlook сами клиенты:

- Точно так же, как клиенты, вы можете создавать экземпляры [контактов](/graph/api/resources/contact) и назначать их объектам [contactFolder](/graph/api/resources/contactfolder).
- API контактов позволяет назначать категории контактам, а также событиям, сообщениям, задачам и записям в группах, чтобы упорядочить эти элементы и упростить их поиск. Кроме того, вы можете [определить основной список категорий пользователя](/graph/api/outlookuser-post-mastercategories), что позволит использовать дополнительные нестандартные сценарии.
- [Контакт](/graph/api/resources/contact) можно пометить для последующего наблюдения. (В настоящее время функция пометки доступна [в предварительной версии ](versioning-and-support.md#beta-version) в Microsoft Graph.)

### <a name="share-contact-information"></a>Общий доступ к информации контактов

API контактов позволяет получать элементы контактов вошедшего пользователя или пользователей, которые поделились своими контактами или делегировали их вошедшему пользователю. Например, если Григорий поделился папкой контактов с Артемом или делегировал доступ к ней, то [делегированные разрешения](auth/auth-concepts.md#microsoft-graph-permissions) от Артема позволят вам читать общие календарь и контент Григория.

### <a name="leverage-people-api-in-microsoft-graph-to-make-better-use-of-all-people-data"></a>Использование API людей в Microsoft Graph для более эффективного использования всех данных пользователей

Вы можете использовать обычные операции CRUD для объекта [contact](/graph/api/resources/contact) Outlook, чтобы создавать контакты и управлять ими. Вы также можете использовать [API людей](people-example.md) в Microsoft Graph, который просматривает контакты Outlook пользователя, а также социальные сети, каталог организации и людей из недавних сообщений и возвращает из этих ресурсов наиболее релевантные сведения о людях для данного пользователя. Используйте эту расширенную аналитику в сценариях с выбором людей.

### <a name="take-advantage-of-other-shared-features-and-conveniences-in-microsoft-graph"></a>Использование преимуществ других общих функций и возможностей в Microsoft Graph

- Объект **contact** поддерживает фотографию контакта, которая реализуется в виде того же объекта [profilePhoto](/graph/api/resources/profilephoto), что и фотография пользователя, хранимая в Exchange Online или Azure Active Directory. Это позволяет исключить потребление ресурсов при преобразовании между фотографией контакта и фотографией профиля пользователя.
- Вы можете синхронизировать локальное хранилище приложения, подписавшись на [уведомления об изменениях](/graph/api/resources/webhooks) и [отслеживание изменений](delta-query-overview.md) в контактах и папках контактов.
- Вы можете увеличить хранилище приложения в экземпляре контакта в виде [открытого расширения](extensibility-overview.md#open-extensions) или добавить строго типизированные пользовательские данные в схему контакта в виде [расширения схемы](extensibility-overview.md#schema-extensions).

## <a name="where-is-the-data"></a>Расположение данных

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API контактов Outlook в Microsoft Graph 1.0](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [API контактов Outlook в бета-версии Microsoft Graph](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и проверьте примеры с запросами контактов в [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fcontacts&version=v1.0). Выберите **Показать другие примеры** в столбце слева. Используйте меню, чтобы включить **Личные контакты**.
- Узнайте, как выполнять указанные ниже действия.
  - [Получение неизменяемых идентификаторов для ресурсов Outlook](outlook-immutable-id.md)
  - [Получение общих контактов](outlook-get-shared-contacts-folders.md)
