---
title: тип перечисления Апплогуплоадстате
description: Апплогуплоадстатус
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ea94f8f8803c268c83d9c6419ad7128339e6d4cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000006"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="59b73-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="59b73-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="59b73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59b73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59b73-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59b73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59b73-106">Апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="59b73-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="59b73-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="59b73-107">Members</span></span>
|<span data-ttu-id="59b73-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="59b73-108">Member</span></span>|<span data-ttu-id="59b73-109">Значение</span><span class="sxs-lookup"><span data-stu-id="59b73-109">Value</span></span>|<span data-ttu-id="59b73-110">Описание</span><span class="sxs-lookup"><span data-stu-id="59b73-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59b73-111">закончен</span><span class="sxs-lookup"><span data-stu-id="59b73-111">pending</span></span>|<span data-ttu-id="59b73-112">нуль</span><span class="sxs-lookup"><span data-stu-id="59b73-112">0</span></span>|<span data-ttu-id="59b73-113">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="59b73-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="59b73-114">готовы</span><span class="sxs-lookup"><span data-stu-id="59b73-114">completed</span></span>|<span data-ttu-id="59b73-115">1,1</span><span class="sxs-lookup"><span data-stu-id="59b73-115">1</span></span>|<span data-ttu-id="59b73-116">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="59b73-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="59b73-117">сбоев</span><span class="sxs-lookup"><span data-stu-id="59b73-117">failed</span></span>|<span data-ttu-id="59b73-118">2</span><span class="sxs-lookup"><span data-stu-id="59b73-118">2</span></span>|<span data-ttu-id="59b73-119">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="59b73-119">Request finished processing and in error state.</span></span>|





