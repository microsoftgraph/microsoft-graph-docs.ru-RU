---
title: Различия в проверке подлинности между Exchange службами (EWS) и Microsoft Graph
description: Описывает сведения о проверке подлинности, чтобы помочь перенести Exchange веб-службы (EWS) в Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 120efa7e2fc4c34b973831131d8fb2c435c2c432
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516575"
---
# <a name="authentication-differences-between-exchange-web-services-ews-and-microsoft-graph"></a>Различия в проверке подлинности между Exchange службами (EWS) и Microsoft Graph

Exchange веб-службы (EWS) и Microsoft Graph используют [платформа удостоверений Майкрософт OAuth 2.0](/azure/active-directory/develop/active-directory-v2-protocols) для проверки подлинности и авторизации.

> [!NOTE]
> В настоящее время EWS также поддерживает базовую проверку подлинности. [Базовая проверка подлинности отключена](/lifecycle/announcements/exchange-online-basic-auth-deprecated) и деактивируется в Microsoft 365 организациях. Microsoft Graph не поддерживает базовую проверку подлинности, поэтому приложения, которые еще не мигрировали в OAuth 2.0, должны сделать это, чтобы получить доступ к Microsoft Graph.

## <a name="permissions"></a>Разрешения

EWS и Microsoft Graph два типа разрешений: делегированная и приложение. Делегированные разрешения находятся в контексте пользователя с проверкой подлинности. Разрешения приложения выданы приложению, которое не действует от имени пользователя.

С помощью EWS приложение имеет доступ ко всему, к чем пользователь имеет доступ (в случае делегирования разрешений) или ко всему, к чем может получить доступ EWS (с разрешениями приложения).

Microsoft Graph предоставляет гранулярные разрешения определенным функциям в Exchange Online почтовом ящике. Например, можно разрешить приложению только читать сообщения почты и не иметь доступа к календарям или контактам. Эффективными разрешениями для делегирования проверки подлинности является пересечение прав пользователя и разрешений, которые были с согласия для приложения. Для проверки подлинности приложений эффективными разрешениями являются набор разрешений, на которые соглашается администратор.

Полный список разрешений, связанных Exchange Microsoft Graph, см. в этой записи:

- [Разрешения почты](permissions-reference.md#mail-permissions)
- [Разрешения календаря](permissions-reference.md#calendars-permissions)
- [Разрешения личных контактов](permissions-reference.md#contacts-permissions)
- [Разрешения для задач](permissions-reference.md#tasks-permissions)

## <a name="impersonation"></a>Олицетворение

[EWS представляет](/exchange/client-developer/exchange-web-services/impersonation-and-ews-in-exchange) собой механизм для приложений EWS, которые работают как учетная запись службы, чтобы выступать в качестве пользователя. Это позволяет приложению принимать действия, например отправку электронной почты, которые, как представляется, приходят от обезличенных пользователей.

В microsoft Graph нет учетных записей служб. Вместо этого разрешения выдают приложениям напрямую. Приложение проверки подлинности с использованием [клиентских учетных данных поток](auth-v2-service.md) со своим удостоверением. По умолчанию согласие администратора предоставляет доступ ко всем почтовым ящикам пользователей, но приложения могут быть ограничены определенными почтовыми [ящиками](auth-limit-mailbox-access.md) администратора.
