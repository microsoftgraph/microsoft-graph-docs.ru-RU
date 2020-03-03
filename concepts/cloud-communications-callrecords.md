---
title: Общие сведения о записях звонков
description: Записи вызовов дают вам информацию о вызовах и собраниях, происходящих в вашей организации.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 4999f4b0d479b6e618055d39a3fecab340deb650
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394643"
---
# <a name="call-records-overview"></a><span data-ttu-id="cf33b-103">Общие сведения о записях звонков</span><span class="sxs-lookup"><span data-stu-id="cf33b-103">Call records overview</span></span>

<span data-ttu-id="cf33b-104">Записи вызовов предоставляют сведения об использовании и диагностике звонков в Организации при использовании Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="cf33b-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="cf33b-105">Данные об использовании и диагностических данных можно использовать для создания настраиваемых отчетов для бизнеса, помогающих отслеживать внедрение или устранять проблемы с качеством звонков.</span><span class="sxs-lookup"><span data-stu-id="cf33b-105">Usage and diagnostic data can be consumed to produce custom reporting for your business to help monitor adoption or to troubleshoot call quality issues.</span></span>

<span data-ttu-id="cf33b-106">Организации могут подписаться на изменения записей вызовов с помощью функции [подписки](/graph/api/resources/webhooks?view=graph-rest-beta) на веб-перехватчик Microsoft Graph, позволяя им создавать отчеты практически в режиме реального времени из данных или для определенных сценариев, таких как экстренные вызовы.</span><span class="sxs-lookup"><span data-stu-id="cf33b-106">Organizations can subscribe to changes to call records using the Microsoft Graph [webhook subscriptions](/graph/api/resources/webhooks?view=graph-rest-beta) capability, allowing them to build near-real-time reports from the data or to alert on certain scenarios like emergency calls.</span></span>

> <span data-ttu-id="cf33b-107">**Важно!** Используйте осторожность при предоставлении разрешений Каллрекордс. Read. ALL приложениям.</span><span class="sxs-lookup"><span data-stu-id="cf33b-107">**Important:** Use discretion when granting the CallRecords.Read.All permission to applications.</span></span> <span data-ttu-id="cf33b-108">Записи звонков могут относиться к операциям бизнеса и, таким образом, могут быть целевыми для злонамеренных субъектов.</span><span class="sxs-lookup"><span data-stu-id="cf33b-108">Call records can provide insights into the operation of your business, and therefore can be a target for malicious actors.</span></span> <span data-ttu-id="cf33b-109">Предоставляйте это разрешение только тем приложениям, которые вы доверяете требованиям к защите данных.</span><span class="sxs-lookup"><span data-stu-id="cf33b-109">Only grant this permission to applications you trust to meet your data protection requirements.</span></span>

## <a name="subscribe-to-call-records"></a><span data-ttu-id="cf33b-110">Подписка на записи звонков</span><span class="sxs-lookup"><span data-stu-id="cf33b-110">Subscribe to call records</span></span>

<span data-ttu-id="cf33b-111">Организации и партнеры часто имеют собственные средства для создания отчетов о вызовах и собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="cf33b-111">Organizations and partners often have their own tooling for generating reports about calls and online meetings.</span></span> <span data-ttu-id="cf33b-112">С помощью веб-перехватчиков они могут получать непрерывный канал записей вызовов по мере их создания.</span><span class="sxs-lookup"><span data-stu-id="cf33b-112">Using webhooks, they can receive a continuous feed of call records as they are created.</span></span> <span data-ttu-id="cf33b-113">Эта модель позволяет организациям и партнерам создавать собственные решения для создания отчетов в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="cf33b-113">This push-model enables organizations and partners to build their own real-time reporting solutions.</span></span>

## <a name="look-up-a-call-record-by-its-call-id"></a><span data-ttu-id="cf33b-114">Поиск записи вызова по ее ИДЕНТИФИКАТОРу вызова</span><span class="sxs-lookup"><span data-stu-id="cf33b-114">Look up a call record by its call ID</span></span>

<span data-ttu-id="cf33b-115">Приложения могут получать [запись вызовов](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="cf33b-115">Applications can retrieve a [call record](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) by its ID.</span></span> <span data-ttu-id="cf33b-116">Этот идентификатор можно определить на основе уведомления веб-перехватчика или получить из средства "Администрирование".</span><span class="sxs-lookup"><span data-stu-id="cf33b-116">This ID can be determined from a webhook notification or retrieved from administrative tools.</span></span>

## <a name="see-also"></a><span data-ttu-id="cf33b-117">См. также</span><span class="sxs-lookup"><span data-stu-id="cf33b-117">See also</span></span>

- [<span data-ttu-id="cf33b-118">Разрешения для записей вызовов</span><span class="sxs-lookup"><span data-stu-id="cf33b-118">Call records permissions</span></span>](/graph/permissions-reference#call-records-permissions)
