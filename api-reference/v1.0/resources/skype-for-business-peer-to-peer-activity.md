---
title: Отчеты об активности в одноранговых сеансах Skype для бизнеса
description: Эти отчеты позволяют получить подробные сведения об активности в одноранговых сеансах Skype для бизнеса в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 895954be67681cdfc0fea0819692f2dca6b874bb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897948"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="5d412-104">Отчеты об активности в одноранговых сеансах Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="5d412-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="5d412-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d412-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d412-106">Эти отчеты позволяют получить подробные сведения об активности в одноранговых сеансах Skype для бизнеса в организации.</span><span class="sxs-lookup"><span data-stu-id="5d412-106">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="5d412-107">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.</span><span class="sxs-lookup"><span data-stu-id="5d412-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="5d412-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти [в статье Microsoft 365 Reports-Peer-to-Peer Activity (Microsoft](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)).</span><span class="sxs-lookup"><span data-stu-id="5d412-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="5d412-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5d412-109">Reports</span></span>

| <span data-ttu-id="5d412-110">Функция</span><span class="sxs-lookup"><span data-stu-id="5d412-110">Function</span></span>                                 | <span data-ttu-id="5d412-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d412-111">Return Type</span></span> | <span data-ttu-id="5d412-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5d412-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="5d412-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="5d412-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="5d412-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5d412-114">Stream</span></span>      | <span data-ttu-id="5d412-115">Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов</span><span class="sxs-lookup"><span data-stu-id="5d412-115">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="5d412-116">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).</span><span class="sxs-lookup"><span data-stu-id="5d412-116">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="5d412-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="5d412-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="5d412-118">Stream</span><span class="sxs-lookup"><span data-stu-id="5d412-118">Stream</span></span>      | <span data-ttu-id="5d412-119">Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="5d412-119">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="5d412-120">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах).</span><span class="sxs-lookup"><span data-stu-id="5d412-120">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="5d412-121">Получение количества минут</span><span class="sxs-lookup"><span data-stu-id="5d412-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="5d412-122">Поток</span><span class="sxs-lookup"><span data-stu-id="5d412-122">Stream</span></span>      | <span data-ttu-id="5d412-123">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="5d412-123">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="5d412-124">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="5d412-124">Types of sessions include audio and video.</span></span> |

