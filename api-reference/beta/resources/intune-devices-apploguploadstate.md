---
title: тип перечисления Апплогуплоадстате
description: апплогуплоадстатус
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ca37de06d50f57eda6c094f195fb5f291181034a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337589"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="cbcae-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="cbcae-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="cbcae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbcae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbcae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbcae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbcae-106">апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="cbcae-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="cbcae-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cbcae-107">Members</span></span>
|<span data-ttu-id="cbcae-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cbcae-108">Member</span></span>|<span data-ttu-id="cbcae-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cbcae-109">Value</span></span>|<span data-ttu-id="cbcae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cbcae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbcae-111">закончен</span><span class="sxs-lookup"><span data-stu-id="cbcae-111">pending</span></span>|<span data-ttu-id="cbcae-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cbcae-112">0</span></span>|<span data-ttu-id="cbcae-113">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="cbcae-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="cbcae-114">готовы</span><span class="sxs-lookup"><span data-stu-id="cbcae-114">completed</span></span>|<span data-ttu-id="cbcae-115">1,1</span><span class="sxs-lookup"><span data-stu-id="cbcae-115">1</span></span>|<span data-ttu-id="cbcae-116">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="cbcae-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="cbcae-117">сбоев</span><span class="sxs-lookup"><span data-stu-id="cbcae-117">failed</span></span>|<span data-ttu-id="cbcae-118">2</span><span class="sxs-lookup"><span data-stu-id="cbcae-118">2</span></span>|<span data-ttu-id="cbcae-119">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="cbcae-119">Request finished processing and in error state.</span></span>|



