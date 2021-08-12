---
title: Обзор API для личных контактов Outlook
description: Контакты Outlook позволяют хранить данные личных контактов и являются частью центра обмена сообщениями Outlook в Microsoft 365. Через Outlook можно управлять сообщениями электронной почты, планировать собрания, искать сведения о пользователях организации, начинать беседы в Интернете, делиться файлами и совместно работать в группах.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 7b8f6eac71265a8fdb71b63d5d01e6d235fb82283dbd02707a8b941f3c7c983e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240382"
---
# <a name="outlook-personal-contacts-api-overview"></a>Обзор API для личных контактов Outlook

Контакты Outlook позволяют хранить данные личных контактов и являются частью центра обмена сообщениями Outlook в Microsoft 365. Через Outlook можно управлять сообщениями электронной почты, планировать собрания, искать сведения о пользователях организации, начинать беседы в Интернете, делиться файлами и совместно работать в группах.

## <a name="why-integrate-with-outlook-personal-contacts"></a>Для чего выполнять интеграцию с личными контактами Outlook?

### <a name="complement-messaging-and-calendaring-scenarios-for-hundreds-of-millions-of-customers"></a>Расширение сценариев обмена сообщениями и ведения календаря для сотен миллионов клиентов

Сотни миллионов потребителей и десятки миллионов организаций выбирают Outlook в качестве своего почтового клиента. Контакты используются как дополнение к обмену сообщениями и ведению календаря, позволяя клиентам хранить данные контактов в Outlook. Для разработчиков, получивших доступ к богатому функционалу [почты](outlook-mail-concept-overview.md) или [календаря](outlook-calendar-concept-overview.md), открывается возможность создания более сложных сценариев с использованием данных о контактах пользователя.

### <a name="automate-contact-organization"></a>Автоматизация организации контактов

API контактов позволяет упорядочивать ваших клиентов аналогично тому, как это делают в Outlook сами клиенты:

- Точно так же, как клиенты, вы можете создавать экземпляры [контактов](/graph/api/resources/contact?view=graph-rest-1.0) и назначать их объектам [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0).
- API контактов позволяет назначать категории контактам, а также событиям, сообщениям, задачам и записям в группах, чтобы упорядочить эти элементы и упростить их поиск. Кроме того, вы можете [определить основной список категорий пользователя](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), что позволит использовать дополнительные нестандартные сценарии.
- [Контакт](/graph/api/resources/contact?view=graph-rest-1.0) можно пометить для последующего наблюдения. (В настоящее время функция пометки доступна [в предварительной версии ](versioning-and-support.md#beta-version) в Microsoft Graph.)

### <a name="share-contact-information"></a>Общий доступ к информации контактов

API контактов позволяет получать элементы контактов вошедшего пользователя или пользователей, которые поделились своими контактами или делегировали их вошедшему пользователю. Например, если Григорий поделился папкой контактов с Артемом или делегировал доступ к ней, то [делегированные разрешения](auth/auth-concepts.md#microsoft-graph-permissions) от Артема позволят вам читать общие календарь и контент Григория.

### <a name="leverage-people-api-in-microsoft-graph-to-make-better-use-of-all-people-data"></a>Использование API людей в Microsoft Graph для более эффективного использования всех данных пользователей

Вы можете использовать обычные операции CRUD для объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0) Outlook, чтобы создавать контакты и управлять ими. Вы также можете использовать [API людей](people-example.md) в Microsoft Graph, который просматривает контакты Outlook пользователя, а также социальные сети, каталог организации и людей из недавних сообщений и возвращает из этих ресурсов наиболее релевантные сведения о людях для данного пользователя. Используйте эту расширенную аналитику в сценариях с выбором людей.

### <a name="take-advantage-of-other-shared-features-and-conveniences-in-microsoft-graph"></a>Использование преимуществ других общих функций и возможностей в Microsoft Graph

- Объект **contact** поддерживает фотографию контакта, которая реализуется в виде того же объекта [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-1.0), что и фотография пользователя, хранимая в Exchange Online или Azure Active Directory. Это позволяет исключить потребление ресурсов при преобразовании между фотографией контакта и фотографией профиля пользователя.
- Вы можете синхронизировать локальное хранилище приложения, подписавшись на [уведомления об изменениях](/graph/api/resources/webhooks?view=graph-rest-1.0) и [отслеживание изменений](delta-query-overview.md) в контактах и папках контактов.
- Вы можете увеличить хранилище приложения в экземпляре контакта в виде [открытого расширения](extensibility-overview.md#open-extensions) или добавить строго типизированные пользовательские данные в схему контакта в виде [расширения схемы](extensibility-overview.md#schema-extensions).

## <a name="where-is-the-data"></a>Расположение данных

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API контактов Outlook в Microsoft Graph 1.0](/graph/api/resources/contact?view=graph-rest-1.0)
- [API контактов Outlook в бета-версии Microsoft Graph](/graph/api/resources/contact?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и проверьте примеры с запросами контактов в [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fcontacts&version=v1.0). Выберите **Показать другие примеры** в столбце слева. Используйте меню, чтобы включить **Личные контакты**.
- Узнайте, как выполнять указанные ниже действия.
  - [Получение неизменяемых идентификаторов для ресурсов Outlook](outlook-immutable-id.md)
  - [Получение общих контактов](outlook-get-shared-contacts-folders.md)
- Ознакомьтесь со справочными материалами по [API контактов](/graph/api/resources/contact?view=graph-rest-1.0) в Outlook.
