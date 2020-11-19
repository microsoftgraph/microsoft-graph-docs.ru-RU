---
title: тип перечисления Апплогуплоадстате
description: апплогуплоадстатус
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2acf8fd19bcbadcbe6cb2371bf357babd4889b7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267847"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="19759-103">тип перечисления Апплогуплоадстате</span><span class="sxs-lookup"><span data-stu-id="19759-103">appLogUploadState enum type</span></span>

<span data-ttu-id="19759-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19759-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19759-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19759-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19759-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19759-107">апплогуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="19759-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="19759-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="19759-108">Members</span></span>
|<span data-ttu-id="19759-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="19759-109">Member</span></span>|<span data-ttu-id="19759-110">Значение</span><span class="sxs-lookup"><span data-stu-id="19759-110">Value</span></span>|<span data-ttu-id="19759-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19759-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19759-112">закончен</span><span class="sxs-lookup"><span data-stu-id="19759-112">pending</span></span>|<span data-ttu-id="19759-113">нуль</span><span class="sxs-lookup"><span data-stu-id="19759-113">0</span></span>|<span data-ttu-id="19759-114">Запрос ожидает обработки или обработки</span><span class="sxs-lookup"><span data-stu-id="19759-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="19759-115">готовы</span><span class="sxs-lookup"><span data-stu-id="19759-115">completed</span></span>|<span data-ttu-id="19759-116">1,1</span><span class="sxs-lookup"><span data-stu-id="19759-116">1</span></span>|<span data-ttu-id="19759-117">Запрос выполнен с помощью файла, отправленного в большой двоичный объект Azure для скачивания.</span><span class="sxs-lookup"><span data-stu-id="19759-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="19759-118">сбоев</span><span class="sxs-lookup"><span data-stu-id="19759-118">failed</span></span>|<span data-ttu-id="19759-119">2</span><span class="sxs-lookup"><span data-stu-id="19759-119">2</span></span>|<span data-ttu-id="19759-120">Запрос завершил обработку и находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="19759-120">Request finished processing and in error state.</span></span>|




