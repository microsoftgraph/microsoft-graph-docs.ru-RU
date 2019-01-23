---
title: Тип перечисления appLogUploadState
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431756"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="06c3e-103">Тип перечисления appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="06c3e-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="06c3e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06c3e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06c3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06c3e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06c3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c3e-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="06c3e-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="06c3e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="06c3e-108">Members</span></span>
|<span data-ttu-id="06c3e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="06c3e-109">Member</span></span>|<span data-ttu-id="06c3e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="06c3e-110">Value</span></span>|<span data-ttu-id="06c3e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="06c3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c3e-112">Ожидание</span><span class="sxs-lookup"><span data-stu-id="06c3e-112">pending</span></span>|<span data-ttu-id="06c3e-113">0</span><span class="sxs-lookup"><span data-stu-id="06c3e-113">0</span></span>|<span data-ttu-id="06c3e-114">Ожидание обработки или в разделе обработки запроса</span><span class="sxs-lookup"><span data-stu-id="06c3e-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="06c3e-115">завершена</span><span class="sxs-lookup"><span data-stu-id="06c3e-115">completed</span></span>|<span data-ttu-id="06c3e-116">1</span><span class="sxs-lookup"><span data-stu-id="06c3e-116">1</span></span>|<span data-ttu-id="06c3e-117">Запрос выполнен с помощью загрузки Azure больших двоичных объектов для загрузки.</span><span class="sxs-lookup"><span data-stu-id="06c3e-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="06c3e-118">failed</span><span class="sxs-lookup"><span data-stu-id="06c3e-118">failed</span></span>|<span data-ttu-id="06c3e-119">2</span><span class="sxs-lookup"><span data-stu-id="06c3e-119">2</span></span>|<span data-ttu-id="06c3e-120">Запрос завершения обработки и состояние ошибки.</span><span class="sxs-lookup"><span data-stu-id="06c3e-120">Request finished processing and in error state.</span></span>|




