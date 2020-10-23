---
title: тип перечисления Апплогуплоадстате
description: апплогуплоадстатус
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fed773a22ba0e538785211ece7849669efd9d383
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725528"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="ed218-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="ed218-103">appLogUploadState enum type</span></span>

<span data-ttu-id="ed218-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed218-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed218-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed218-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed218-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed218-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed218-107">апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="ed218-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="ed218-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ed218-108">Members</span></span>
|<span data-ttu-id="ed218-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ed218-109">Member</span></span>|<span data-ttu-id="ed218-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ed218-110">Value</span></span>|<span data-ttu-id="ed218-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed218-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed218-112">закончен</span><span class="sxs-lookup"><span data-stu-id="ed218-112">pending</span></span>|<span data-ttu-id="ed218-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ed218-113">0</span></span>|<span data-ttu-id="ed218-114">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="ed218-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="ed218-115">готовы</span><span class="sxs-lookup"><span data-stu-id="ed218-115">completed</span></span>|<span data-ttu-id="ed218-116">1,1</span><span class="sxs-lookup"><span data-stu-id="ed218-116">1</span></span>|<span data-ttu-id="ed218-117">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="ed218-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="ed218-118">сбоев</span><span class="sxs-lookup"><span data-stu-id="ed218-118">failed</span></span>|<span data-ttu-id="ed218-119">2</span><span class="sxs-lookup"><span data-stu-id="ed218-119">2</span></span>|<span data-ttu-id="ed218-120">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="ed218-120">Request finished processing and in error state.</span></span>|





