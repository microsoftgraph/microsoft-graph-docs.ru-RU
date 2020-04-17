---
title: Пределы API облачных коммуникаций в Microsoft Graph
description: Содержит сведения о пределах API облачных коммуникаций
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 0338c7b37a58da66aac75430234a4b1df56b07b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871667"
---
# <a name="cloud-communication-api-limits-in-microsoft-graph"></a><span data-ttu-id="4425a-103">Пределы API облачных коммуникаций в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4425a-103">Cloud communication API limits in Microsoft Graph</span></span>

<span data-ttu-id="4425a-104">В этой статье описываются ограничения API облачных коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="4425a-104">This article describes limitations to the cloud communications APIs.</span></span> <span data-ttu-id="4425a-105">Эти пределы помогают обеспечить стабильность, надежность и безопасность платформы.</span><span class="sxs-lookup"><span data-stu-id="4425a-105">These limits help to ensure that the platform is stable, reliable, and secure.</span></span> <span data-ttu-id="4425a-106">Обратите внимание на то, что эти ограничения могут быть изменены в будущем.</span><span class="sxs-lookup"><span data-stu-id="4425a-106">Note that these limitations are subject to change in the future.</span></span> 

><span data-ttu-id="4425a-107">**Примечание:** При достижении предельного значения попытка увеличить количество запросов API приведет к появлению HTTP `429 Error`-запроса.</span><span class="sxs-lookup"><span data-stu-id="4425a-107">**Note:** When the limit is reached, attempting to make more API requests will result in an HTTP `429 Error`.</span></span>

| <span data-ttu-id="4425a-108">API</span><span class="sxs-lookup"><span data-stu-id="4425a-108">API</span></span>      | <span data-ttu-id="4425a-109">Ограничения</span><span class="sxs-lookup"><span data-stu-id="4425a-109">Limitations</span></span>    |
| :------------- | :----------: |
|  <span data-ttu-id="4425a-110">Звонки</span><span class="sxs-lookup"><span data-stu-id="4425a-110">Calls</span></span> | <span data-ttu-id="4425a-111">10 000 звонков/мес и 100 одновременные вызовы</span><span class="sxs-lookup"><span data-stu-id="4425a-111">10,000 calls/month and 100 concurrent calls</span></span>   |
| <span data-ttu-id="4425a-112">Собрания</span><span class="sxs-lookup"><span data-stu-id="4425a-112">Meetings</span></span>   | <span data-ttu-id="4425a-113">2000 собраний и пользователей в месяц</span><span class="sxs-lookup"><span data-stu-id="4425a-113">2000 meetings/user each month</span></span> |
| <span data-ttu-id="4425a-114">Присутствие (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4425a-114">Presence (preview)</span></span>   | <span data-ttu-id="4425a-115">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="4425a-115">2 requests/second</span></span> |

## <a name="see-also"></a><span data-ttu-id="4425a-116">См. также</span><span class="sxs-lookup"><span data-stu-id="4425a-116">See also</span></span>

- [<span data-ttu-id="4425a-117">Работа с API Communications</span><span class="sxs-lookup"><span data-stu-id="4425a-117">Working with the communications API</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-beta)
