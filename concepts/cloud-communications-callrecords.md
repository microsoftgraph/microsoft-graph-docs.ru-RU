---
title: Общие сведения о записях звонков
description: Записи вызовов дают вам информацию о вызовах и собраниях, происходящих в вашей организации.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 43d41184bbb2af9c63b2818f91ef578579df4119
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509597"
---
# <a name="call-records-overview"></a><span data-ttu-id="f06f0-103">Общие сведения о записях звонков</span><span class="sxs-lookup"><span data-stu-id="f06f0-103">Call records overview</span></span>

<span data-ttu-id="f06f0-104">Записи звонков содержат сведения об использовании и диагностике, касающиеся звонков и собраний по сети в вашей организации при применении Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f06f0-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="f06f0-105">Данные об использовании и диагностических данных можно использовать для создания настраиваемых отчетов для бизнеса, помогающих отслеживать внедрение или устранять проблемы с качеством звонков.</span><span class="sxs-lookup"><span data-stu-id="f06f0-105">Usage and diagnostic data can be consumed to produce custom reporting for your business to help monitor adoption or to troubleshoot call quality issues.</span></span>

<span data-ttu-id="f06f0-106">Организации могут подписаться на изменения записей вызовов с помощью функции [подписки](/graph/api/resources/webhooks?view=graph-rest-1.0) на веб-перехватчик Microsoft Graph, позволяя им создавать отчеты практически в режиме реального времени из данных или для определенных сценариев, таких как экстренные вызовы.</span><span class="sxs-lookup"><span data-stu-id="f06f0-106">Organizations can subscribe to changes to call records using the Microsoft Graph [webhook subscriptions](/graph/api/resources/webhooks?view=graph-rest-1.0) capability, allowing them to build near-real-time reports from the data or to alert on certain scenarios like emergency calls.</span></span>

> <span data-ttu-id="f06f0-107">**Важно!** Используйте осторожность при предоставлении разрешений Каллрекордс. Read. ALL приложениям.</span><span class="sxs-lookup"><span data-stu-id="f06f0-107">**Important:** Use discretion when granting the CallRecords.Read.All permission to applications.</span></span> <span data-ttu-id="f06f0-108">Записи звонков могут относиться к операциям бизнеса и, таким образом, могут быть целевыми для злонамеренных субъектов.</span><span class="sxs-lookup"><span data-stu-id="f06f0-108">Call records can provide insights into the operation of your business, and therefore can be a target for malicious actors.</span></span> <span data-ttu-id="f06f0-109">Предоставляйте это разрешение только приложениям, которым вы доверяете в плане соблюдения ваших требований к защите данных.</span><span class="sxs-lookup"><span data-stu-id="f06f0-109">Only grant this permission to applications you trust to meet your data protection requirements.</span></span>

## <a name="subscribe-to-call-records"></a><span data-ttu-id="f06f0-110">Подписка на записи звонков</span><span class="sxs-lookup"><span data-stu-id="f06f0-110">Subscribe to call records</span></span>

<span data-ttu-id="f06f0-111">Организации и партнеры часто имеют собственные средства для создания отчетов о вызовах и собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="f06f0-111">Organizations and partners often have their own tooling for generating reports about calls and online meetings.</span></span> <span data-ttu-id="f06f0-112">С помощью веб-перехватчиков они могут получать непрерывный канал записей вызовов по мере их создания.</span><span class="sxs-lookup"><span data-stu-id="f06f0-112">Using webhooks, they can receive a continuous feed of call records as they are created.</span></span> <span data-ttu-id="f06f0-113">Эта модель позволяет организациям и партнерам создавать собственные решения для создания отчетов в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="f06f0-113">This push-model enables organizations and partners to build their own real-time reporting solutions.</span></span>

## <a name="look-up-a-call-record-by-its-call-id"></a><span data-ttu-id="f06f0-114">Поиск записи вызова по ее ИДЕНТИФИКАТОРу вызова</span><span class="sxs-lookup"><span data-stu-id="f06f0-114">Look up a call record by its call ID</span></span>

<span data-ttu-id="f06f0-115">Приложения могут получать [запись вызовов](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f06f0-115">Applications can retrieve a [call record](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) by its ID.</span></span> <span data-ttu-id="f06f0-116">Этот идентификатор можно определить на основе уведомления веб-перехватчика или получить из средства "Администрирование".</span><span class="sxs-lookup"><span data-stu-id="f06f0-116">This ID can be determined from a webhook notification or retrieved from administrative tools.</span></span>

## <a name="get-call-record-reports"></a><span data-ttu-id="f06f0-117">Получение отчетов о записи вызовов</span><span class="sxs-lookup"><span data-stu-id="f06f0-117">Get call record reports</span></span>

<span data-ttu-id="f06f0-118">Организации, которые используют Microsoft Teams для подключения к телефонной сети общего пользования (PSTN), обычно заключают отслеживание этих сведений об использовании, чтобы получить представление о связанных затратах.</span><span class="sxs-lookup"><span data-stu-id="f06f0-118">Organizations that use Microsoft Teams to connect to the public switched telephone network (PSTN) usually want to track this usage to understand the associated costs.</span></span> <span data-ttu-id="f06f0-119">Функции [жетпстнкаллс](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) и [жетдиректраутингкаллс](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) возвращают проекцию данных [записи вызовов](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) в табличном формате.</span><span class="sxs-lookup"><span data-stu-id="f06f0-119">The [getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) and [getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) functions return a projection of [call record](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) data in a tabular format.</span></span>

## <a name="see-also"></a><span data-ttu-id="f06f0-120">Дополнительные ресурсы:</span><span class="sxs-lookup"><span data-stu-id="f06f0-120">See also</span></span>

- [<span data-ttu-id="f06f0-121">Разрешения для записей звонков</span><span class="sxs-lookup"><span data-stu-id="f06f0-121">Call records permissions</span></span>](/graph/permissions-reference#call-records-permissions)
