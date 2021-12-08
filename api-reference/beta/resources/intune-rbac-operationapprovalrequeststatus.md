---
title: тип enum operationApprovalRequestStatus
description: Состояние текущего запроса на утверждение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b60e9071de452cdf42a8ef58246be77bdfd868a8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342239"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>тип enum operationApprovalRequestStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние текущего запроса на утверждение

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный статус|
|needsApproval|1|Запрос на утверждение требует утверждения перед тем, как действие может быть завершено.|
|утверждено|2|Запрос на утверждение утвержден, действие теперь можно завершить.|
|отклонено|3|Запрос на утверждение отклонен, действие не утверждено и никаких дальнейших действий не может быть принято.|
|отменено|4|Запрос на утверждение, отмененный пользователем, не требующий дальнейших действий.|
|завершено|5|Запрос на утверждение завершен, не требуя дальнейших действий.|
|истек срок действия|6 |Срок действия запроса на утверждение истек, для выполнения этого запроса необходимо сделать новое утверждение.|




