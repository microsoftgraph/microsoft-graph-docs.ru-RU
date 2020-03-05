---
title: тип перечисления Апплогуплоадстате
description: апплогуплоадстатус
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d692e352f177c7f882a33e49604934c4b1a22912
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525168"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="20705-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="20705-103">appLogUploadState enum type</span></span>

<span data-ttu-id="20705-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="20705-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20705-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20705-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20705-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20705-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20705-107">апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="20705-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="20705-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="20705-108">Members</span></span>
|<span data-ttu-id="20705-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="20705-109">Member</span></span>|<span data-ttu-id="20705-110">Значение</span><span class="sxs-lookup"><span data-stu-id="20705-110">Value</span></span>|<span data-ttu-id="20705-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20705-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20705-112">закончен</span><span class="sxs-lookup"><span data-stu-id="20705-112">pending</span></span>|<span data-ttu-id="20705-113">нуль</span><span class="sxs-lookup"><span data-stu-id="20705-113">0</span></span>|<span data-ttu-id="20705-114">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="20705-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="20705-115">готовы</span><span class="sxs-lookup"><span data-stu-id="20705-115">completed</span></span>|<span data-ttu-id="20705-116">1 </span><span class="sxs-lookup"><span data-stu-id="20705-116">1</span></span>|<span data-ttu-id="20705-117">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="20705-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="20705-118">сбоев</span><span class="sxs-lookup"><span data-stu-id="20705-118">failed</span></span>|<span data-ttu-id="20705-119">2 </span><span class="sxs-lookup"><span data-stu-id="20705-119">2</span></span>|<span data-ttu-id="20705-120">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="20705-120">Request finished processing and in error state.</span></span>|



