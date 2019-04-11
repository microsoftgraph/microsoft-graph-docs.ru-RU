---
title: тип перечисления Апплогуплоадстате
description: Апплогуплоадстатус
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b59210e7a00fde1e62e1cbc056f0bd34625330e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792736"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="82dff-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="82dff-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="82dff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82dff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82dff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82dff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82dff-106">Апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="82dff-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="82dff-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="82dff-107">Members</span></span>
|<span data-ttu-id="82dff-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="82dff-108">Member</span></span>|<span data-ttu-id="82dff-109">Значение</span><span class="sxs-lookup"><span data-stu-id="82dff-109">Value</span></span>|<span data-ttu-id="82dff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="82dff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82dff-111">закончен</span><span class="sxs-lookup"><span data-stu-id="82dff-111">pending</span></span>|<span data-ttu-id="82dff-112">нуль</span><span class="sxs-lookup"><span data-stu-id="82dff-112">0</span></span>|<span data-ttu-id="82dff-113">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="82dff-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="82dff-114">готовы</span><span class="sxs-lookup"><span data-stu-id="82dff-114">completed</span></span>|<span data-ttu-id="82dff-115">1,1</span><span class="sxs-lookup"><span data-stu-id="82dff-115">1</span></span>|<span data-ttu-id="82dff-116">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="82dff-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="82dff-117">сбоев</span><span class="sxs-lookup"><span data-stu-id="82dff-117">failed</span></span>|<span data-ttu-id="82dff-118">2</span><span class="sxs-lookup"><span data-stu-id="82dff-118">2</span></span>|<span data-ttu-id="82dff-119">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="82dff-119">Request finished processing and in error state.</span></span>|





