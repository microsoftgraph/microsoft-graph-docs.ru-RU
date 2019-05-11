---
title: тип перечисления Апплогуплоадстате
description: Апплогуплоадстатус
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6a0c880fe8fa7fe743bea3ad42fee6d1e24d209
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943118"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="da039-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="da039-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="da039-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da039-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da039-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da039-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da039-106">Апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="da039-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="da039-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="da039-107">Members</span></span>
|<span data-ttu-id="da039-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="da039-108">Member</span></span>|<span data-ttu-id="da039-109">Значение</span><span class="sxs-lookup"><span data-stu-id="da039-109">Value</span></span>|<span data-ttu-id="da039-110">Описание</span><span class="sxs-lookup"><span data-stu-id="da039-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da039-111">закончен</span><span class="sxs-lookup"><span data-stu-id="da039-111">pending</span></span>|<span data-ttu-id="da039-112">нуль</span><span class="sxs-lookup"><span data-stu-id="da039-112">0</span></span>|<span data-ttu-id="da039-113">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="da039-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="da039-114">готовы</span><span class="sxs-lookup"><span data-stu-id="da039-114">completed</span></span>|<span data-ttu-id="da039-115">1,1</span><span class="sxs-lookup"><span data-stu-id="da039-115">1</span></span>|<span data-ttu-id="da039-116">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="da039-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="da039-117">сбоев</span><span class="sxs-lookup"><span data-stu-id="da039-117">failed</span></span>|<span data-ttu-id="da039-118">2</span><span class="sxs-lookup"><span data-stu-id="da039-118">2</span></span>|<span data-ttu-id="da039-119">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="da039-119">Request finished processing and in error state.</span></span>|




