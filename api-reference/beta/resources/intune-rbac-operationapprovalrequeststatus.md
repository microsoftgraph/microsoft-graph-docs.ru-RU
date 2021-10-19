---
title: тип enum operationApprovalRequestStatus
description: Состояние текущего запроса на утверждение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22053b80a983af725720aa5fe11e8e93176cea49
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494417"
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
|отменено|4 |Запрос на утверждение, отмененный пользователем, не требующий дальнейших действий.|
|завершено|5|Запрос на утверждение завершен, не требуя дальнейших действий.|
|истек срок действия|6 |Срок действия запроса на утверждение истек, для выполнения этого запроса необходимо сделать новое утверждение.|



