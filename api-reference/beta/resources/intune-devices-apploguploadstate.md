---
title: тип перечисления Апплогуплоадстате
description: апплогуплоадстатус
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 193344351f5654ea09c0246e06d1d3abf0d54039
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785135"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="7db92-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="7db92-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="7db92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7db92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7db92-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7db92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7db92-106">апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="7db92-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="7db92-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7db92-107">Members</span></span>
|<span data-ttu-id="7db92-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7db92-108">Member</span></span>|<span data-ttu-id="7db92-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7db92-109">Value</span></span>|<span data-ttu-id="7db92-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7db92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7db92-111">закончен</span><span class="sxs-lookup"><span data-stu-id="7db92-111">pending</span></span>|<span data-ttu-id="7db92-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7db92-112">0</span></span>|<span data-ttu-id="7db92-113">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="7db92-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="7db92-114">готовы</span><span class="sxs-lookup"><span data-stu-id="7db92-114">completed</span></span>|<span data-ttu-id="7db92-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7db92-115">1</span></span>|<span data-ttu-id="7db92-116">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="7db92-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="7db92-117">сбоев</span><span class="sxs-lookup"><span data-stu-id="7db92-117">failed</span></span>|<span data-ttu-id="7db92-118">2</span><span class="sxs-lookup"><span data-stu-id="7db92-118">2</span></span>|<span data-ttu-id="7db92-119">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="7db92-119">Request finished processing and in error state.</span></span>|



