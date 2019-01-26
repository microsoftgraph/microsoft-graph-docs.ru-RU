---
title: Отчеты об активности в одноранговых сеансах Skype для бизнеса
description: Подробные сведения можно получить в действии peer-to-peer внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8802430e6f2725b520e7b558f48ed760c26b7588
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572418"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="b5607-104">Отчеты об активности в одноранговых сеансах Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b5607-104">Skype for Business peer-to-peer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5607-105">Подробные сведения можно получить в действии peer-to-peer внутри организации.</span><span class="sxs-lookup"><span data-stu-id="b5607-105">You can get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="b5607-106">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.</span><span class="sxs-lookup"><span data-stu-id="b5607-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="b5607-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="b5607-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="b5607-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="b5607-108">Reports</span></span>

| <span data-ttu-id="b5607-109">Функция</span><span class="sxs-lookup"><span data-stu-id="b5607-109">Function</span></span>                                 | <span data-ttu-id="b5607-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="b5607-110">CSV return type</span></span> | <span data-ttu-id="b5607-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="b5607-111">JSON return type</span></span>                         | <span data-ttu-id="b5607-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b5607-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b5607-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="b5607-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="b5607-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b5607-114">Stream</span></span>          | [<span data-ttu-id="b5607-115">skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b5607-115">skypeForBusinessPeerToPeerActivityCounts</span></span>](../resources/skypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="b5607-116">Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов</span><span class="sxs-lookup"><span data-stu-id="b5607-116">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="b5607-117">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).</span><span class="sxs-lookup"><span data-stu-id="b5607-117">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="b5607-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b5607-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="b5607-119">Stream</span><span class="sxs-lookup"><span data-stu-id="b5607-119">Stream</span></span>          | [<span data-ttu-id="b5607-120">skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b5607-120">skypeForBusinessPeerToPeerActivityUserCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="b5607-121">Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="b5607-121">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="b5607-122">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах).</span><span class="sxs-lookup"><span data-stu-id="b5607-122">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="b5607-123">Получение количества минут</span><span class="sxs-lookup"><span data-stu-id="b5607-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="b5607-124">Поток</span><span class="sxs-lookup"><span data-stu-id="b5607-124">Stream</span></span>          | [<span data-ttu-id="b5607-125">skypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="b5607-125">skypeForBusinessPeerToPeerActivityMinuteCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="b5607-126">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="b5607-126">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="b5607-127">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="b5607-127">Types of sessions include audio and video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-peer-to-peer-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
