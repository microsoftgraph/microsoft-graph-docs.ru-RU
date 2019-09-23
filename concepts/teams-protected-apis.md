---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: cf8f977d2a8d8e9e9704118718ac0c8da9b6ae77
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036321"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="22391-103">Защищенные API в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="22391-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="22391-104">API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.</span><span class="sxs-lookup"><span data-stu-id="22391-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="22391-105">Перед использованием этих API необходимо выполнить дополнительные проверки, кроме проверки разрешений и согласия.</span><span class="sxs-lookup"><span data-stu-id="22391-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="22391-106">В настоящий момент защищенными являются следующие API:</span><span class="sxs-lookup"><span data-stu-id="22391-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="22391-107">[Перечисление сообщений в каналах](/graph/api/channel-list-messages?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="22391-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="22391-108">[Получение сообщений в каналах](/graph/api/channel-get-message?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="22391-108">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="22391-109">[Перечисление ответов на сообщение](/graph/api/channel-list-messagereplies?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="22391-109">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="22391-110">[Получение ответа на сообщение](/graph/api/channel-get-messagereply?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="22391-110">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="22391-111">[Перечисление сообщений в чате](/graph/api/chatmessage-list?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="22391-111">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="22391-112">[Получение сообщения в чате](/graph/api/chatmessage-get?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="22391-112">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

>[!NOTE]
><span data-ttu-id="22391-113">[Отправка сообщения](/graph/api/channel-post-messages?view=graph-rest-beta) не является защищенным API.</span><span class="sxs-lookup"><span data-stu-id="22391-113">[Send message](/graph/api/channel-post-messages?view=graph-rest-beta) is not a protected API.</span></span>

<span data-ttu-id="22391-114">Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](http://aka.ms/teamsgraph/requestaccess).</span><span class="sxs-lookup"><span data-stu-id="22391-114">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="22391-115">Мы просматриваем запросы на доступ каждую среду и выпускаем утверждения каждую пятницу.</span><span class="sxs-lookup"><span data-stu-id="22391-115">We review access requests every Wednesday and deploy approvals every Friday.</span></span>
<span data-ttu-id="22391-116">Если вы хотите предоставить информацию в дополнение к форме, обратитесь по адресу [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="22391-116">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>
