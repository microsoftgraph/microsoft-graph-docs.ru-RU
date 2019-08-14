---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 124a2f96f2c59909311fad605beeb1273193d8af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364532"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="c3c15-103">Защищенные API в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c3c15-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="c3c15-104">API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.</span><span class="sxs-lookup"><span data-stu-id="c3c15-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="c3c15-105">Перед использованием этих API необходимо выполнить дополнительные проверки, кроме проверки разрешений и согласия.</span><span class="sxs-lookup"><span data-stu-id="c3c15-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="c3c15-106">В настоящий момент защищенными являются следующие API:</span><span class="sxs-lookup"><span data-stu-id="c3c15-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="c3c15-107">[Перечисление сообщений в каналах](/graph/api/channel-list-messages?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="c3c15-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="c3c15-108">[Получение сообщений в каналах](/graph/api/channel-get-message?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="c3c15-108">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="c3c15-109">[Перечисление ответов на сообщение](/graph/api/channel-list-messagereplies?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="c3c15-109">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="c3c15-110">[Получение ответа на сообщение](/graph/api/channel-get-messagereply?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="c3c15-110">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="c3c15-111">[Перечисление сообщений в чате](/graph/api/chatmessage-list?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="c3c15-111">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="c3c15-112">[Получение сообщения в чате](/graph/api/chatmessage-get?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="c3c15-112">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

<span data-ttu-id="c3c15-113">Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](http://aka.ms/teamsgraph/requestaccess).</span><span class="sxs-lookup"><span data-stu-id="c3c15-113">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="c3c15-114">Мы просматриваем запросы на доступ каждую среду и выпускаем утверждения каждую пятницу.</span><span class="sxs-lookup"><span data-stu-id="c3c15-114">We review access requests every Wednesday and deploy approvals every Friday.</span></span>
<span data-ttu-id="c3c15-115">Если вы хотите предоставить информацию в дополнение к форме, обратитесь по адресу [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c3c15-115">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>
