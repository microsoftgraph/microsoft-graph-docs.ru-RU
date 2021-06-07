---
title: тип enum defenderCloudBlockLevelType
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: edc8f58be9c9bfdce904988503b42e20ed2d0bfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755891"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="f5a86-103">тип enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="f5a86-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="f5a86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5a86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5a86-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5a86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5a86-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="f5a86-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="f5a86-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f5a86-107">Members</span></span>
|<span data-ttu-id="f5a86-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f5a86-108">Member</span></span>|<span data-ttu-id="f5a86-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f5a86-109">Value</span></span>|<span data-ttu-id="f5a86-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5a86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5a86-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f5a86-111">notConfigured</span></span>|<span data-ttu-id="f5a86-112">0</span><span class="sxs-lookup"><span data-stu-id="f5a86-112">0</span></span>|<span data-ttu-id="f5a86-113">Значение по умолчанию, использует уровень антивирусная программа по умолчанию и обеспечивает сильное обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="f5a86-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="f5a86-114">высокая</span><span class="sxs-lookup"><span data-stu-id="f5a86-114">high</span></span>|<span data-ttu-id="f5a86-115">1</span><span class="sxs-lookup"><span data-stu-id="f5a86-115">1</span></span>|<span data-ttu-id="f5a86-116">High применяет высокий уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="f5a86-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="f5a86-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="f5a86-117">highPlus</span></span>|<span data-ttu-id="f5a86-118">2</span><span class="sxs-lookup"><span data-stu-id="f5a86-118">2</span></span>|<span data-ttu-id="f5a86-119">High + использует высокий уровень и применяет меры защиты от добавления</span><span class="sxs-lookup"><span data-stu-id="f5a86-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="f5a86-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="f5a86-120">zeroTolerance</span></span>|<span data-ttu-id="f5a86-121">3</span><span class="sxs-lookup"><span data-stu-id="f5a86-121">3</span></span>|<span data-ttu-id="f5a86-122">Нулевая толерантность блокирует все неизвестные исполняемые</span><span class="sxs-lookup"><span data-stu-id="f5a86-122">Zero tolerance blocks all unknown executables</span></span>|




