---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ebf0bbda324f62c6413bbe3d70ade33a5052da0d
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778763"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="cf7a8-103">Защищенные API в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cf7a8-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="cf7a8-104">API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="cf7a8-105">Перед использованием этих API необходимо выполнить дополнительные проверки, за пределами разрешений и согласия.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="cf7a8-106">В настоящий момент защищенными являются следующие API:</span><span class="sxs-lookup"><span data-stu-id="cf7a8-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="cf7a8-107">[Перечисление сообщений в каналах](/graph/api/channel-list-messages?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="cf7a8-108">[Получение сообщений в каналах](/graph/api/channel-get-message?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-108">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="cf7a8-109">[Перечисление ответов на сообщение](/graph/api/channel-list-messagereplies?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-109">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="cf7a8-110">[Получение ответа на сообщение](/graph/api/channel-get-messagereply?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-110">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="cf7a8-111">[Перечисление сообщений в чате](/graph/api/chatmessage-list?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-111">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="cf7a8-112">[Получение сообщения в чате](/graph/api/chatmessage-get?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-112">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

<span data-ttu-id="cf7a8-113">Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](http://aka.ms/teamsgraph/requestaccess).</span><span class="sxs-lookup"><span data-stu-id="cf7a8-113">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="cf7a8-114">Мы еженедельно просматривая запросы на доступ.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-114">We review access requests weekly.</span></span> <span data-ttu-id="cf7a8-115">Если вы хотите предоставить информацию в дополнение к форме, обратитесь по адресу [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="cf7a8-115">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>
