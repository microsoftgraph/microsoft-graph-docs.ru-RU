---
title: тип перечисления Апплогуплоадстате
description: апплогуплоадстатус
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f3a39e8155c6cb18291ee233574c592f3ce964ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060835"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="2fa2d-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="2fa2d-103">appLogUploadState enum type</span></span>

<span data-ttu-id="2fa2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fa2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fa2d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fa2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fa2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fa2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fa2d-107">апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="2fa2d-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="2fa2d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2fa2d-108">Members</span></span>
|<span data-ttu-id="2fa2d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2fa2d-109">Member</span></span>|<span data-ttu-id="2fa2d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2fa2d-110">Value</span></span>|<span data-ttu-id="2fa2d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa2d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa2d-112">закончен</span><span class="sxs-lookup"><span data-stu-id="2fa2d-112">pending</span></span>|<span data-ttu-id="2fa2d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2fa2d-113">0</span></span>|<span data-ttu-id="2fa2d-114">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="2fa2d-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="2fa2d-115">готовы</span><span class="sxs-lookup"><span data-stu-id="2fa2d-115">completed</span></span>|<span data-ttu-id="2fa2d-116">1 </span><span class="sxs-lookup"><span data-stu-id="2fa2d-116">1</span></span>|<span data-ttu-id="2fa2d-117">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="2fa2d-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="2fa2d-118">сбоев</span><span class="sxs-lookup"><span data-stu-id="2fa2d-118">failed</span></span>|<span data-ttu-id="2fa2d-119">2 </span><span class="sxs-lookup"><span data-stu-id="2fa2d-119">2</span></span>|<span data-ttu-id="2fa2d-120">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="2fa2d-120">Request finished processing and in error state.</span></span>|






